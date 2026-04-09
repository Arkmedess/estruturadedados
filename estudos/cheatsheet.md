# Cheat Sheet de Prova - Estrutura de Dados

## O que mais pode cair
1. Diferenca entre lista, tupla, set e dicionario.
2. Metodos de lista: append, insert, remove, pop, sort.
3. Funcoes com return, parametro padrao, *args, **kwargs.
4. Lambda com map e filter.
5. NumPy: shape, ndim, size e operacao vetorizada.
6. Pandas: Series x DataFrame e filtro.
7. Pilha (LIFO), Fila (FIFO) e Lista Encadeada.

## Estruturas basicas (resposta em 1 linha)
- Lista: mutavel, ordenada, aceita duplicatas.
- Tupla: imutavel, ordenada, aceita duplicatas.
- Set: mutavel, nao ordenado, sem duplicatas.
- Dicionario: chave-valor, busca por chave.

## Sintaxe que voce precisa lembrar

### Lista
- `lista = [1, 2, 3]`
- `lista[0]`, `lista[-1]`, `lista[1:3]`
- `lista.append(x)`, `lista.insert(i, x)`, `lista.remove(x)`, `lista.pop()`, `lista.sort()`

### Tupla
- `tupla = (1, 2, 3)`

### Set
- `s = {1, 2, 2, 3}`  -> remove duplicatas automaticamente
- `a | b`, `a & b`, `a - b`, `a ^ b`

### Dicionario
- `d = {'nome': 'Ana', 'idade': 25}`
- `d['nome']`, `d['idade'] = 26`, `del d['idade']`

### *args e **kwargs
```python
def f(*args, **kwargs):
    print(args)
    print(kwargs)
```

### Lambda
- `lambda x, y: x + y`
- `list(map(lambda x: x * 2, [1, 2, 3]))`
- `list(filter(lambda x: x % 2 == 0, [1, 2, 3, 4]))`

## NumPy (direto ao ponto)
- `v = np.array([1, 2, 3])`
- `m = np.array([[1, 2], [3, 4]])`
- `m.shape` (formato), `m.ndim` (dimensoes), `m.size` (total elementos)
- `v * 2` (vetorizacao sem loop)

## Pandas (direto ao ponto)
- `s = pd.Series([10, 20, 30])`
- `df = pd.DataFrame({'nome': ['Ana', 'Beto'], 'idade': [25, 30]})`
- `df['nome']` (coluna)
- `df[df['idade'] > 26]` (filtro)
- Series = 1 coluna | DataFrame = tabela

## Pilha, Fila e Lista Encadeada
- Pilha (LIFO): ultimo entra, primeiro sai.
- Fila (FIFO): primeiro entra, primeiro sai.
- Lista Encadeada: no com dado + referencia para o proximo no.

## Perguntas e respostas curtas de prova
1. Lista x Tupla? Lista e mutavel; tupla e imutavel.
2. Por que usar set? Para eliminar duplicatas e fazer operacoes de conjunto.
3. Para que serve **kwargs? Receber argumentos nomeados variaveis.
4. O que e shape no NumPy? Formato do array.
5. Series x DataFrame? Coluna unica x tabela 2D.
6. Pilha x Fila? LIFO x FIFO.

## Checklist final de 1 minuto
- Sei diferenciar lista, tupla, set e dicionario.
- Sei usar append, pop, remove, sort.
- Sei usar return, *args, **kwargs e lambda.
- Sei ler shape, ndim e size.
- Sei diferenciar Series e DataFrame.
- Sei explicar LIFO e FIFO.
