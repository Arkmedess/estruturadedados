# Instalacao Rapida no Windows (venv)

Este guia foi feito para quem vai receber o projeto em ZIP e usar no Windows.

## Requisitos
- Python 3.12 ou superior instalado
- PowerShell

## 0) Confirmar Python no Windows
No PowerShell, rode:

```powershell
py --version
```

Se esse comando falhar, instale o Python e marque a opcao de adicionar ao PATH.

## 1) Entrar na pasta do projeto

```powershell
cd C:\caminho\para\estruturadedados
```

## 2) Criar o ambiente virtual

```powershell
py -3 -m venv .venv
```

## 3) Ativar o ambiente virtual

```powershell
.\.venv\Scripts\Activate.ps1
```

Se aparecer erro de politica de execucao, rode este comando e tente ativar de novo:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```

## 4) Instalar dependencias

```powershell
python -m pip install --upgrade pip
pip install -r requirements.txt
```

## 5) Registrar kernel do Jupyter

```powershell
python -m ipykernel install --user --name estruturadedados-venv --display-name "Python (estruturadedados-venv)"
```

## 6) Abrir a cola de prova

```powershell
jupyter lab estudos/cola_prova.ipynb
```

## 7) Selecionar kernel no VS Code/Jupyter
Escolha o kernel:

- Python (estruturadedados-venv)

## Comandos rapidos para o dia a dia

Ativar ambiente:

```powershell
.\.venv\Scripts\Activate.ps1
```

Desativar ambiente:

```powershell
deactivate
```

## Opcional: fluxo com uv no Windows

```powershell
uv sync --dev
uv run jupyter lab estudos/cola_prova.ipynb
```
