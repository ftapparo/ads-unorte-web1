# Aula 3: Listas e Tabelas em HTML

## Introdução

Nesta aula, você aprenderá a criar listas e tabelas em HTML. Listas são úteis para organizar informações de forma sequencial, enquanto tabelas são usadas para exibir dados em formato estruturado, facilitando a leitura e a compreensão.

## Tipos de Listas em HTML

Existem dois tipos principais de listas em HTML: **Listas Ordenadas** e **Listas Não Ordenadas**.

### Listas Ordenadas (`<ol>`)

As listas ordenadas utilizam números para indicar a sequência dos itens.

```html
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ol>

```

### Listas Não Ordenadas (`<ul>`)

As listas não ordenadas utilizam marcadores (bullets) ao invés de números.

```html
<ul>
    <li>Item A</li>
    <li>Item B</li>
    <li>Item C</li>
</ul>

```

### Listas Não Ordenadas (`<ul>`)

As listas não ordenadas utilizam marcadores (bullets) ao invés de números.

```html
<ul>
    <li>Item A</li>
    <li>Item B
        <ul>
            <li>Subitem B1</li>
            <li>Subitem B2</li>
        </ul>
    </li>
    <li>Item C</li>
</ul>

```

## Tabelas em HTML

As tabelas em HTML são usadas para organizar dados em linhas e colunas. Aqui estão as principais tags utilizadas para criar tabelas:

- **`<table>`**: Define o início e o fim da tabela.
- **`<tr>`**: Define uma linha da tabela.
- **`<td>`**: Define uma célula de dados (coluna) em uma linha.
- **`<th>`**: Define o cabeçalho de uma coluna (negrito e centralizado por padrão).

### Exemplo de Tabela Simples

```html
<table>
    <tr>
        <th>Nome</th>
        <th>Idade</th>
        <th>Cidade</th>
    </tr>
    <tr>
        <td>Ana</td>
        <td>25</td>
        <td>São Paulo</td>
    </tr>
    <tr>
        <td>Carlos</td>
        <td>30</td>
        <td>Rio de Janeiro</td>
    </tr>
</table>

```

### Atributos de Tabelas

Você pode estilizar e modificar a aparência das tabelas usando atributos como `border`, `colspan`, `rowspan`, e `cellspacing`.

- **`border`**: Adiciona uma borda à tabela e suas células.
- **`colspan`**: Permite que uma célula ocupe várias colunas.
- **`rowspan`**: Permite que uma célula ocupe várias linhas.

### Exemplo de Tabela com Atributos

```html
<table border="1">
    <tr>
        <th colspan="2">Nome Completo</th>
        <th>Idade</th>
    </tr>
    <tr>
        <td>Ana</td>
        <td>Santos</td>
        <td>25</td>
    </tr>
    <tr>
        <td>Carlos</td>
        <td>Silva</td>
        <td rowspan="2">30</td>
    </tr>
    <tr>
        <td>Beatriz</td>
        <td>Souza</td>
    </tr>
</table>

```

## Exercício Prático

1. Crie uma página HTML que contenha:
   - Uma **lista ordenada** com pelo menos três itens.
   - Uma **lista não ordenada** com subitens (listas aninhadas).
   - Uma tabela simples que mostre o nome, idade e cidade de três pessoas.

---

### Estrutura Sugerida

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Exemplo de Listas e Tabelas</title>
</head>
<body>
    <h1>Exemplo de Listas</h1>

    <h2>Lista Ordenada</h2>
    <ol>
        <li>Primeiro Item</li>
        <li>Segundo Item</li>
        <li>Terceiro Item</li>
    </ol>

    <h2>Lista Não Ordenada</h2>
    <ul>
        <li>Item A</li>
        <li>Item B
            <ul>
                <li>Subitem B1</li>
                <li>Subitem B2</li>
            </ul>
        </li>
    </ul>

    <h1>Exemplo de Tabela</h1>
    <table border="1">
        <tr>
            <th>Nome</th>
            <th>Idade</th>
            <th>Cidade</th>
        </tr>
        <tr>
            <td>Ana</td>
            <td>25</td>
            <td>São Paulo</td>
        </tr>
        <tr>
            <td>Carlos</td>
            <td>30</td>
            <td>Rio de Janeiro</td>
        </tr>
    </table>
</body>
</html>

```
