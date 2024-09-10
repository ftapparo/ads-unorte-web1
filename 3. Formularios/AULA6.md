# Aula 6: Estilizando Formulários com CSS

## Introdução

Nesta aula, você aprenderá como usar CSS para melhorar a aparência e a usabilidade de formulários em suas páginas HTML. Estilizar formulários é essencial para proporcionar uma experiência de usuário agradável e profissional.

## Aplicando Estilos Básicos

Você pode aplicar estilos diretamente aos elementos de formulário, como campos de texto, áreas de texto, botões, etc., utilizando seletores do CSS.

### Exemplo de Estilo Básico

```html
<style>
    input, textarea {
        width: 100%;
        padding: 10px;
        margin-bottom: 10px;
        border: 1px solid #ccc;
        border-radius: 4px;
        font-size: 16px;
    }

    button {
        background-color: #4CAF50;
        color: white;
        padding: 10px 20px;
        border: none;
        border-radius: 4px;
        cursor: pointer;
        font-size: 16px;
    }

    button:hover {
        background-color: #45a049;
    }
</style>
```
Esse código aplica estilos consistentes aos campos de entrada, áreas de texto e botões.

---

## Estilos para Campos de Formulário

Você pode definir diferentes estilos para cada tipo de campo de formulário, como campos de texto, e-mails, e áreas de texto.

### Exemplo: Estilos Diferenciados para Campos de Texto e Áreas de Texto

```html
<style>
    input[type="text"], input[type="email"], textarea {
        width: 100%;
        padding: 10px;
        margin-bottom: 15px;
        border: 2px solid #ddd;
        border-radius: 5px;
        font-size: 16px;
    }

    input[type="text"]:focus, input[type="email"]:focus, textarea:focus {
        border-color: #4CAF50;
        outline: none;
    }
</style>
```

- **`input[type="text"]`**: Aplica estilo aos campos de texto.
- **`input`**: Aplica estilo quando o campo está em foco (quando o usuário clica no campo).


---

## Estilos para Botões

Os botões são uma parte fundamental dos formulários, e sua estilização pode melhorar a experiência de interação.

### Exemplo de Estilo para Botões

```html
<style>
    button {
        background-color: #008CBA;
        color: white;
        padding: 15px 20px;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        font-size: 16px;
    }

    button:hover {
        background-color: #006f9b;
    }

    button:active {
        background-color: #005f8a;
    }
</style>
```

- **`button:hover`**: Aplica um efeito ao passar o mouse sobre o botão.
- **`button:active`**: Aplica um estilo quando o botão é clicado.


---

## Estilizando o Placeholder

O placeholder é o texto de exemplo que aparece dentro dos campos de formulário antes do usuário inserir os dados. Você pode personalizar a aparência desse texto.

### Exemplo de Estilo para Placeholder

```html
<style>
    ::placeholder {
        color: #888;
        font-style: italic;
    }

    input:focus::placeholder {
        color: #ccc;
    }
</style>
```

Esse estilo define uma cor cinza e itálico para o placeholder e muda sua cor quando o campo está em foco.

---

## Layout Flexível com CSS Grid e Flexbox

CSS Grid e Flexbox são duas ferramentas poderosas para criar layouts responsivos e organizados para formulários.

### Exemplo de Formulário com CSS Grid

```html
<style>
    form {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 20px;
    }

    label, input, textarea {
        width: 100%;
    }

    .full-width {
        grid-column: span 2;
    }
</style>

<form>
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome">

    <label for="email">E-mail:</label>
    <input type="email" id="email" name="email">

    <label for="mensagem" class="full-width">Mensagem:</label>
    <textarea id="mensagem" name="mensagem" class="full-width"></textarea>

    <button type="submit" class="full-width">Enviar</button>
</form>
```
Esse exemplo cria um layout de formulário com duas colunas, usando CSS Grid.


---

## Exercício Prático

1. Crie um formulário com os seguintes elementos:
   - Campos de texto e e-mail.
   - Uma área de texto.
   - Um botão de envio.
   - Personalize a aparência do formulário usando CSS.

---

### Estrutura Sugerida

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Formulário Estilizado</title>
    <style>
        input, textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            font-size: 16px;
        }

        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }

        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <h1>Formulário de Contato</h1>
    <form>
        <label for="nome">Nome:</label>
        <input type="text" id="nome" name="nome" placeholder="Digite seu nome" required>

        <label for="email">E-mail:</label>
        <input type="email" id="email" name="email" placeholder="Digite seu e-mail" required>

        <label for="mensagem">Mensagem:</label>
        <textarea id="mensagem" name="mensagem" placeholder="Escreva sua mensagem" required></textarea>

        <button type="submit">Enviar</button>
    </form>
</body>
</html>
```