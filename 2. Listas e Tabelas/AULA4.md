# Aula 4: Tabelas em HTML

## Introdução

Nesta aula, você aprenderá sobre a criação de tabelas em HTML. As tabelas são utilizadas para organizar e exibir dados de forma estruturada em linhas e colunas. Veremos a estrutura básica de uma tabela e como usar as principais tags de tabelas.

## Estrutura Básica de Tabelas

A estrutura de uma tabela em HTML é composta pelas seguintes tags principais:

- **`<table>`**: Define o início e o fim de uma tabela.
- **`<tr>`**: Define uma linha da tabela.
- **`<td>`**: Define uma célula de dados em uma linha.
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

---

## Atributos de Tabelas

As tabelas em HTML podem ser estilizadas e organizadas usando diversos atributos. Vamos ver os principais:

- **`border`**: Define uma borda para a tabela e as células.
- **`colspan`**: Permite que uma célula ocupe várias colunas.
- **`rowspan`**: Permite que uma célula ocupe várias linhas.
- **`cellpadding`**: Define o espaçamento interno das células.

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

---

## Estilizando Tabelas com CSS

Você pode aplicar estilos às tabelas para melhorar sua aparência e tornar os dados mais fáceis de visualizar.

### Exemplo de Estilização de Tabelas

```html
<style>
    table {
        width: 100%;
        border-collapse: collapse;
    }
    
    th, td {
        padding: 10px;
        text-align: left;
        border-bottom: 1px solid #ddd;
    }

    th {
        background-color: #f4f4f4;
    }
</style>

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

---

## Exercício Prático

1. Crie uma página HTML que contenha uma tabela com os seguintes dados:
   - Nome
   - Idade
   - Cidade
   - Use pelo menos 3 linhas e 3 colunas.

2. Adicione uma borda à tabela e estilize as células usando CSS.

---

### Estrutura Sugerida

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Tabela de Usuários</title>
    <style>
        table {
            width: 100%;
            border-collapse: collapse;
        }
        
        th, td {
            padding: 10px;
            border: 1px solid #ccc;
            text-align: left;
        }

        th {
            background-color: #f4f4f4;
        }
    </style>
</head>
<body>
    <h1>Tabela de Usuários</h1>
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
        <tr>
            <td>Beatriz</td>
            <td>22</td>
            <td>Belo Horizonte</td>
        </tr>
    </table>
</body>
</html>
```