# Aula 7: Validação Básica de Formulários em HTML

## Introdução

Nesta aula, você aprenderá como validar formulários em HTML utilizando atributos básicos. A validação de formulários garante que os dados inseridos pelo usuário sigam certas regras antes de serem enviados, prevenindo erros e melhorando a coleta de informações.

## Validação Básica com Atributos HTML

O HTML oferece vários atributos para garantir que os dados sejam inseridos corretamente antes de enviar o formulário. Vamos explorar os atributos mais utilizados para validação básica:

- **`required`**: Torna o campo obrigatório.
- **`minlength` e `maxlength`**: Define o número mínimo e máximo de caracteres.
- **`min` e `max`**: Define o valor mínimo e máximo para números ou datas.
- **`pattern`**: Usa expressões regulares para validar padrões específicos.

## Exemplo de Validação com HTML

Aqui está um exemplo de como usar esses atributos para validar um formulário simples:

```html
<form action="URL_destino" method="POST">
    <label for="nome">Nome (obrigatório):</label>
    <input type="text" id="nome" name="nome" required><br><br>

    <label for="email">E-mail (obrigatório e com formato de e-mail):</label>
    <input type="email" id="email" name="email" required><br><br>

    <label for="senha">Senha (mínimo de 8 caracteres):</label>
    <input type="password" id="senha" name="senha" minlength="8" required><br><br>

    <label for="idade">Idade (entre 18 e 100):</label>
    <input type="number" id="idade" name="idade" min="18" max="100" required><br><br>

    <button type="submit">Enviar</button>
</form>
```

---

## Validação com o Atributo `pattern`

O atributo `pattern` permite criar validações personalizadas usando expressões regulares. Ele é especialmente útil quando você precisa validar padrões específicos, como números de telefone ou códigos postais.

### Exemplo de Validação com `pattern`

```html
<form action="URL_destino" method="POST">
    <label for="telefone">Telefone (formato: (99) 99999-9999):</label>
    <input type="tel" id="telefone" name="telefone" pattern="\\(\\d{2}\\) \\d{5}-\\d{4}" placeholder="(99) 99999-9999" required><br><br>

    <button type="submit">Enviar</button>
</form>
```

---

## Mensagens de Erro Padrão

Quando a validação do formulário falha, o navegador exibe mensagens de erro padrão para ajudar o usuário a corrigir as informações. Você pode personalizar essas mensagens utilizando o atributo `title`.

### Exemplo de Mensagem de Erro Personalizada

```html
<form action="URL_destino" method="POST">
    <label for="senha">Senha (mínimo de 8 caracteres):</label>
    <input type="password" id="senha" name="senha" minlength="8" required title="A senha deve ter pelo menos 8 caracteres"><br><br>

    <button type="submit">Enviar</button>
</form>
```

---

## Exercício Prático

1. Crie um formulário HTML que inclua os seguintes campos:
   - Nome (obrigatório).
   - E-mail (obrigatório e com validação de formato).
   - Senha (mínimo de 8 caracteres).
   - Idade (número entre 18 e 100).
   - Telefone (validação com `pattern` para o formato `(99) 99999-9999`).

---

### Estrutura Sugerida

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Formulário com Validação</title>
</head>
<body>
    <h1>Formulário de Cadastro</h1>
    <form action="URL_destino" method="POST">
        <label for="nome">Nome (obrigatório):</label>
        <input type="text" id="nome" name="nome" required><br><br>

        <label for="email">E-mail (obrigatório):</label>
        <input type="email" id="email" name="email" required><br><br>

        <label for="senha">Senha (mínimo de 8 caracteres):</label>
        <input type="password" id="senha" name="senha" minlength="8" required><br><br>

        <label for="idade">Idade (entre 18 e 100):</label>
        <input type="number" id="idade" name="idade" min="18" max="100" required><br><br>

        <label for="telefone">Telefone (formato: (99) 99999-9999):</label>
        <input type="tel" id="telefone" name="telefone" pattern="\\(\\d{2}\\) \\d{5}-\\d{4}" placeholder="(99) 99999-9999" required><br><br>

        <button type="submit">Enviar</button>
    </form>
</body>
</html>
```
