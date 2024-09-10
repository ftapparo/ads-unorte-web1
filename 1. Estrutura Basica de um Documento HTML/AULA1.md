# Aula 1: Estrutura Básica de um Documento HTML

## Introdução

Nesta aula, você aprenderá sobre a estrutura básica de um documento HTML e como utilizar as principais tags essenciais para a construção de uma página web simples. O HTML (HyperText Markup Language) é a base de qualquer página web e define a estrutura e o conteúdo visualizado no navegador.

## Estrutura Básica de um Documento HTML

Todo documento HTML começa e termina com as tags `<html>`. Dentro desta estrutura, existem dois principais blocos: `<head>` e `<body>`.

### Exemplo de Estrutura Básica

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Título da Página</title>
</head>
<body>
    <h1>Bem-vindo ao HTML!</h1>
    <p>Este é um exemplo básico de uma estrutura HTML.</p>
</body>
</html>

```
### Explicação das Tags

**`<!DOCTYPE html>`**: Informa ao navegador que o documento está utilizando a versão HTML5.
**`<html lang="pt-BR">`**: Inicia o documento HTML e define o idioma como português brasileiro.
**`<head>`**: Contém metadados sobre a página, como título, codificação de caracteres e links para estilos.
**`<meta charset="UTF-8">`**: Define a codificação de caracteres para UTF-8, suportando caracteres especiais.
**`<title>`**: Define o título da página, que aparece na aba do navegador.
**`<body>`**: Contém o conteúdo visível da página, como textos, imagens, links, etc.

## Detalhamento dos Elementos

### 1. **DOCTYPE**

- O `<!DOCTYPE html>` é uma declaração obrigatória que indica ao navegador que o documento usa HTML5, garantindo que a página seja renderizada corretamente.

### 2. **`<html>`**

- A tag `<html>` é o contêiner raiz de todo o documento HTML. Tudo que está entre as tags `<html>` e `</html>` faz parte do conteúdo da página.

### 3. **`<head>`**

- O bloco `<head>` contém informações sobre a página, como o título, metadados e links para recursos externos (CSS, scripts, etc.), mas nada dentro de `<head>` é visível no corpo da página.

### 4. **`<meta charset="UTF-8">`**

- O meta charset define a codificação de caracteres como UTF-8, permitindo a exibição correta de caracteres especiais, como acentos e símbolos.

### 5. **`<title>`**

- O título da página definido pela tag `<title>` é o texto que aparece na aba do navegador quando a página é carregada.

### 6. **`<body>`**

- O `<body>` é onde todo o conteúdo visível da página é inserido, como textos, imagens, vídeos, e outros elementos HTML.

## Exercício Prático

Crie um documento HTML com a seguinte estrutura:

1. Um título adequado para a página.
2. Um cabeçalho `<h1>` com o texto "Minha Primeira Página Web".
3. Um parágrafo `<p>` descrevendo o que você espera aprender no curso de desenvolvimento web.

---

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Minha Primeira Página Web</title>
</head>
<body>
    <h1>Minha Primeira Página Web</h1>
    <p>Estou empolgado para aprender sobre HTML, CSS e desenvolvimento web. Espero criar páginas interativas e funcionais.</p>
</body>
</html>
```
