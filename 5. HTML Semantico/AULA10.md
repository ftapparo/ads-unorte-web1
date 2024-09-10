# Aula 10: HTML Semântico e Suas Tags

## Introdução

Nesta aula, vamos aprender sobre as **tags semânticas** do HTML. O HTML semântico melhora a acessibilidade e o SEO (Otimização para Motores de Busca), além de tornar a estrutura do conteúdo mais clara e organizada. As tags semânticas ajudam os navegadores e os motores de busca a entenderem o propósito de cada parte da página.

## O Que é HTML Semântico?

O HTML semântico utiliza tags que indicam claramente o propósito do conteúdo, como artigos, seções, rodapés e navegação. Essas tags ajudam a estruturar o conteúdo de forma que seja fácil de entender, tanto para humanos quanto para máquinas.

### Principais Tags Semânticas

- **`<article>`**: Representa um conteúdo independente, como um artigo ou post.
- **`<section>`**: Define uma seção genérica do conteúdo.
- **`<header>`**: Representa o cabeçalho de uma página ou de uma seção.
- **`<footer>`**: Representa o rodapé de uma página ou de uma seção.
- **`<nav>`**: Indica uma área de navegação com links.
- **`<aside>`**: Representa conteúdo complementar, como barras laterais.

### Exemplo de Estrutura Semântica

```html
<header>
    <h1>Título da Página</h1>
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Sobre</a></li>
            <li><a href="#">Contato</a></li>
        </ul>
    </nav>
</header>

<section>
    <article>
        <h2>Artigo 1</h2>
        <p>Este é o conteúdo do primeiro artigo.</p>
    </article>

    <article>
        <h2>Artigo 2</h2>
        <p>Este é o conteúdo do segundo artigo.</p>
    </article>
</section>

<aside>
    <h3>Barra Lateral</h3>
    <p>Este é o conteúdo complementar.</p>
</aside>

<footer>
    <p>&copy; 2024 Meu Site</p>
</footer>
```

---

## Benefícios do HTML Semântico

O uso de tags semânticas oferece diversos benefícios tanto para desenvolvedores quanto para usuários e motores de busca.

### 1. **Acessibilidade**

As tags semânticas tornam as páginas mais acessíveis, especialmente para usuários com deficiências que utilizam leitores de tela. Um leitor de tela pode identificar facilmente onde está o conteúdo principal, menus de navegação, rodapés e outras partes da página.

### 2. **SEO (Otimização para Motores de Busca)**

Os motores de busca, como o Google, dão preferência a páginas que utilizam HTML semântico. Ao entender a estrutura e o conteúdo da página, os motores de busca podem indexá-la melhor, o que melhora o ranking da página nos resultados de busca.

### 3. **Clareza na Estrutura**

O HTML semântico ajuda a manter o código mais organizado e claro. Tanto os desenvolvedores quanto os navegadores podem compreender a função de cada parte da página com mais facilidade, o que facilita a manutenção e o desenvolvimento futuro.

---

## Principais Tags Semânticas em Detalhe

### 1. **`<article>`**

Representa um conteúdo independente que pode ser distribuído ou republicado fora do contexto original, como artigos, blogs ou postagens.

### 2. **`<section>`**

Uma seção genérica de um documento que agrupa conteúdo relacionado. Geralmente, cada seção tem um título (`<h1>`, `<h2>`, etc.).

### 3. **`<header>`**

Define o cabeçalho da página ou de uma seção. Pode conter logotipos, menus de navegação, títulos e outros elementos introdutórios.

### 4. **`<footer>`**

Define o rodapé da página ou de uma seção. Contém informações como direitos autorais, links para políticas, ou outras informações finais.

### 5. **`<nav>`**

Define uma área de navegação, geralmente contendo links para outras partes do site ou para outras páginas.

### 6. **`<aside>`**

Representa conteúdo relacionado ao principal, como barras laterais com anúncios, links ou informações extras.

## Exercício Prático

1. Crie uma página HTML utilizando as seguintes tags semânticas:
   - Um **`<header>`** com um título e uma barra de navegação.
   - Uma **`<section>`** com dois artigos (**`<article>`**), cada um com um título e parágrafos de conteúdo.
   - Um **`<aside>`** com conteúdo adicional.
   - Um **`<footer>`** com informações de rodapé.

---

### Estrutura Sugerida

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Página Semântica</title>
</head>
<body>
    <header>
        <h1>Minha Página Semântica</h1>
        <nav>
            <ul>
                <li><a href="#">Início</a></li>
                <li><a href="#">Sobre</a></li>
                <li><a href="#">Contato</a></li>
            </ul>
        </nav>
    </header>

    <section>
        <article>
            <h2>Primeiro Artigo</h2>
            <p>Este é o conteúdo do primeiro artigo.</p>
        </article>

        <article>
            <h2>Segundo Artigo</h2>
            <p>Este é o conteúdo do segundo artigo.</p>
        </article>
    </section>

    <aside>
        <h3>Barra Lateral</h3>
        <p>Informações complementares ou links importantes.</p>
    </aside>

    <footer>
        <p>&copy; 2024 Meu Site. Todos os direitos reservados.</p>
    </footer>
</body>
</html>
```
