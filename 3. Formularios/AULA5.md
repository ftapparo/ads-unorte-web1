# Aula 5: Formulários em HTML

## Introdução

Nesta aula, você aprenderá como criar e utilizar formulários em HTML. Formulários são essenciais para interagir com os usuários e coletar informações, permitindo o envio de dados para processamento. Veremos as principais tags e atributos que compõem os formulários.

## Estrutura de um Formulário

A tag `<form>` é utilizada para definir o início e o fim de um formulário. Dentro dela, colocamos os campos para coleta de dados, como `<input>`, `<textarea>`, e `<button>`.

### Estrutura Básica de um Formulário

```html
<form action="URL_destino" method="POST">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome">
    <button type="submit">Enviar</button>
</form>
```

### Atributos Principais do (`<form>`)

- **action**: Define o URL para onde os dados do formulário serão enviados.
- **method**: Define o método HTTP de envio. Comumente usado: POST ou GET.

---

## Tipos de Campos de Formulário

O HTML oferece diversos tipos de campos para coleta de dados. Vamos explorar alguns dos principais:

- **Textual**:
    - `<input type="text">`: Campo de texto padrão.
    - `<textarea>`: Área de texto para inserção de múltiplas linhas.

- **Seleção**:
    - `<input type="radio">`: Botão de seleção única.
    - `<input type="checkbox">`: Caixa de seleção múltipla.
    - `<select>` e `<option>`: Menu suspenso.

- **Outros Tipos**:
    - `<input type="email">`: Campo de e-mail.
    - `<input type="password">`: Campo de senha.
    - `<input type="submit">`: Botão de envio.

### Exemplo de Formulário com Vários Tipos de Campos

```html
<form action="URL_destino" method="POST">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome"><br><br>

    <label for="email">E-mail:</label>
    <input type="email" id="email" name="email"><br><br>

    <label for="mensagem">Mensagem:</label>
    <textarea id="mensagem" name="mensagem"></textarea><br><br>

    <label for="sexo">Sexo:</label><br>
    <input type="radio" id="masculino" name="sexo" value="masculino"> Masculino<br>
    <input type="radio" id="feminino" name="sexo" value="feminino"> Feminino<br><br>

    <label for="interesses">Interesses:</label><br>
    <input type="checkbox" id="esportes" name="interesses" value="esportes"> Esportes<br>
    <input type="checkbox" id="musica" name="interesses" value="musica"> Música<br><br>

    <button type="submit">Enviar</button>
</form>
```

---

## Atributos de Campos de Formulário

Cada campo de formulário pode ter diferentes atributos para melhorar a funcionalidade e validação. Alguns dos atributos mais comuns incluem:

- **required**: Campo obrigatório.
- **placeholder**: Texto de exemplo que aparece dentro do campo.
- **maxlength**: Limita o número de caracteres no campo.
- **min** e **max**: Define limites numéricos ou de data.

### Exemplo com Atributos

```html
<form action="URL_destino" method="POST">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome" placeholder="Digite seu nome" required><br><br>

    <label for="idade">Idade:</label>
    <input type="number" id="idade" name="idade" min="18" max="100"><br><br>

    <button type="submit">Enviar</button>
</form>
```

---

## Métodos de Envio: GET e POST

Os formulários podem ser enviados utilizando dois métodos principais: **GET** e **POST**.

- **GET**: Os dados são enviados como parâmetros na URL, e geralmente é usado para buscas ou envio de dados não sensíveis.
  
- **POST**: Os dados são enviados no corpo da requisição HTTP, tornando-o mais seguro para enviar informações sensíveis, como senhas.

### Exemplo de Formulário usando GET

```html
<form action="/buscar" method="GET">
    <label for="consulta">Buscar:</label>
    <input type="text" id="consulta" name="consulta">
    <button type="submit">Pesquisar</button>
</form>
```

---

## Exercício Prático

1. Crie um formulário HTML que inclua os seguintes campos:
   - Nome (campo de texto).
   - E-mail (campo de e-mail).
   - Mensagem (área de texto).
   - Opções de seleção (radio buttons e checkboxes).
   - Um botão de envio.

---

### Estrutura Sugerida

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Formulário de Contato</title>
</head>
<body>
    <h1>Formulário de Contato</h1>
    <form action="URL_destino" method="POST">
        <label for="nome">Nome:</label>
        <input type="text" id="nome" name="nome" required><br><br>

        <label for="email">E-mail:</label>
        <input type="email" id="email" name="email" required><br><br>

        <label for="mensagem">Mensagem:</label>
        <textarea id="mensagem" name="mensagem" required></textarea><br><br>

        <label for="sexo">Sexo:</label><br>
        <input type="radio" id="masculino" name="sexo" value="masculino"> Masculino<br>
        <input type="radio" id="feminino" name="sexo" value="feminino"> Feminino<br><br>

        <label for="interesses">Interesses:</label><br>
        <input type="checkbox" id="esportes" name="interesses" value="esportes"> Esportes<br>
        <input type="checkbox" id="musica" name="interesses" value="musica"> Música<br><br>

        <button type="submit">Enviar</button>
    </form>
</body>
</html>
```


