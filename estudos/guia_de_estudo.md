# Guia de Estudo - Estrutura de Dados

## Objetivo
Este guia reúne os pontos principais dos notebooks da disciplina para servir como material de consulta em provas.

## Como usar este material
1. Leia cada seção abaixo para entender o conceito.
2. Abra o notebook correspondente em `Notebooks/` sempre que precisar de exemplos ou código.
3. Use `cheatsheet.md` como referência rápida durante revisões.

## 1. Conceitos básicos de Estrutura de Dados
- Estrutura de Dados (ED) organiza e armazena informações de forma eficiente.
- ED impactam diretamente o desempenho de algoritmos.
- Em Ciência de Dados, entender ED ajuda a manipular coleções e processar dados corretamente.

## 2. Tipos de estruturas de dados em Python
### Listas
- Mutáveis e ordenadas.
- Aceitam elementos duplicados.
- Uso comum: coleção de itens que pode crescer e mudar.
- Principais métodos: `append`, `extend`, `insert`, `remove`, `pop`, `sort`, `reverse`, `index`, `count`.

### Tuplas
- Imutáveis e ordenadas.
- Usadas quando não se quer que os dados sejam alterados.
- Exemplo: coordenadas, configurações fixas.

### Sets (conjuntos)
- Não mantêm ordem.
- Não aceitam duplicatas.
- Bons para operações de conjunto: união, interseção, diferença.

### Dicionários (contexto geral)
- Estrutura chave-valor.
- Permite acesso rápido por chave.
- Relacionado ao conteúdo de `**kwargs` explicado no material extra.

## 3. Pandas: Series e DataFrame
### Series
- Estrutura unidimensional rotulada.
- Semelhante a uma lista com índice.
- Permite operações vetorizadas e alinhamento automático.

### DataFrame
- Estrutura bidimensional em forma de tabela.
- Cada coluna pode ter tipo diferente.
- Uso comum: análise de dados tabulares, transformação e limpeza.

### Quando usar
- `Series`: uma única coluna de dados com índice.
- `DataFrame`: tabela completa com várias colunas e linhas.

## 4. Funções e argumentos em Python
### `lambda`
- Função anônima de uma linha.
- Boa para operações simples e rápidas.
- Exemplos comuns: `lambda x: x + 1`, `lambda x: 'Par' if x % 2 == 0 else 'Ímpar'`.

### `*args` e `**kwargs`
- `*args`: recebe argumentos posicionais variáveis.
- `**kwargs`: recebe argumentos nomeados em forma de dicionário.
- Útil para criar funções flexíveis que não sabem quantos parâmetros receberão.

## 5. Plano de estudo recomendado
1. Comece por `Notebooks/Estrutura_de_Dados_Aula_01.ipynb`: listas, tuplas e sets.
2. Avance para os notebooks seguintes, focando em cada tema apresentado.
3. Leia `Notebooks/Estrutura_de_Dados_EXTRA_01.ipynb` para consolidar `lambda` e `**kwargs`.
4. Pratique executando os exemplos no próprio notebook.
5. Use este guia e `cheatsheet.md` para revisão rápida antes da prova.

## 6. Dicas para prova
- Explique as diferenças entre listas, tuplas e sets.
- Mostre exemplos de métodos básicos em listas.
- Compare `Series` e `DataFrame` com exemplos simples.
- Demonstre o uso de `lambda` em `map`, `filter` ou listas por compreensão.
- Se precisar escrever função, use `**kwargs` quando a assinatura deve aceitar parâmetros nomeados variáveis.
