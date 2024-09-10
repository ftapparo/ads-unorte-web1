# Aula 2: Formatação de Texto e Inserção de Links e Imagens

## Introdução

Nesta aula, você aprenderá como formatar texto em HTML utilizando diferentes tags e como inserir links e imagens em suas páginas. A formatação de texto ajuda a organizar e destacar partes importantes de seu conteúdo, enquanto os links e as imagens tornam sua página interativa e visualmente atraente.

## Formatação de Texto

HTML oferece diversas tags para formatar o texto de acordo com a necessidade. Aqui estão as principais:

- **`<h1>` a `<h6>`**: Define títulos, do mais importante (`<h1>`) ao menos importante (`<h6>`).
- **`<p>`**: Define um parágrafo.
- **`<strong>`**: Destaca um texto em negrito.
- **`<em>`**: Destaca um texto em itálico.
- **`<br>`**: Insere uma quebra de linha.
- **`<hr>`**: Insere uma linha horizontal.

### Exemplo de Formatação de Texto

```html
<h1>Título de Nível 1</h1>
<p>Este é um parágrafo com <strong>texto em negrito</strong> e <em>texto em itálico</em>.</p>
<br>
<p>Esta é uma nova linha após a quebra.</p>
<hr>
<p>Após a linha horizontal.</p>
```

---

## Inserção de Links

A tag `<a>` é usada para criar links em HTML. Você pode criar links para outras páginas, sites externos ou até âncoras dentro da própria página.

### Estrutura Básica

```html
<a href="URL do destino">Texto do Link</a>
<a href="https://www.google.com">Visite o Google</a>
<a href="#secao2">Ir para a Seção 2 desta página</a>
```

---

## Inserção de Imagens

A tag `<img>` é usada para inserir imagens em uma página HTML. Ao contrário de outras tags, `<img>` é uma tag auto-fechada, ou seja, não tem uma tag de fechamento.

### Estrutura Básica

```html
<img src="URL da Imagem" alt="Descrição da Imagem">
<img src="https://www.exemplo.com/imagem.jpg" alt="Exemplo de Imagem">
```
---

## Exercício Prático

Crie um documento HTML que inclua:

1. Um título `<h1>` e um subtítulo `<h2>`.
2. Dois parágrafos com texto, onde um contenha **negrito** e outro **itálico**.
3. Um link para o site da sua escolha.
4. Uma imagem usando o atributo `src` com uma URL de sua escolha.

---

### Estrutura Sugerida

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Minha Página com Formatação de Texto</title>
</head>
<body>
    <h1>Bem-vindo à Minha Página</h1>
    <h2>Formatação de Texto e Links</h2>
    <p>Este é um parágrafo com <strong>texto em negrito</strong>.</p>
    <p>Este é outro parágrafo com <em>texto em itálico</em>.</p>
    <a href="https://www.exemplo.com">Clique aqui para visitar um site</a>
    <br>
    <img src="https://www.exemplo.com/imagem.jpg" alt="Descrição da Imagem">
</body>
</html>
```

