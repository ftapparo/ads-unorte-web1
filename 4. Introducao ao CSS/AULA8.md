# Aula 8: Estilos Básicos para Textos e Elementos em CSS

## Introdução

Nesta aula, você aprenderá a aplicar estilos básicos em textos e outros elementos de uma página HTML utilizando CSS. Vamos explorar propriedades como fontes, cores, espaçamento (padding e margin), bordas e alinhamento de texto.

## Estilizando Textos com CSS

O CSS oferece diversas propriedades para estilizar textos, tornando seu conteúdo mais atraente e legível. Algumas das propriedades mais comuns para textos são:

- **`font-family`**: Define a fonte usada no texto.
- **`font-size`**: Define o tamanho da fonte.
- **`font-weight`**: Define a espessura do texto (normal, bold, etc.).
- **`color`**: Define a cor do texto.
- **`text-align`**: Define o alinhamento do texto (esquerda, direita, centro, ou justificado).

### Exemplo de Estilo de Texto

```css
p {
    font-family: Arial, sans-serif;
    font-size: 16px;
    font-weight: normal;
    color: #333;
    text-align: justify;
}
```

---

## Estilizando Fontes com CSS

A propriedade **`font-family`** define a fonte utilizada nos textos da página. É uma boa prática definir fontes alternativas (fallback) para o caso de a fonte primária não estar disponível no navegador do usuário.

### Exemplo de Uso de `font-family`

```css
h1 {
    font-family: "Helvetica", "Arial", sans-serif;
}
```

---

## Estilizando Cores com CSS

A propriedade **`color`** é usada para definir a cor do texto. As cores podem ser especificadas em diferentes formatos, como:

- **Nomes de cores**: `color: red;`
- **Códigos hexadecimais**: `color: #ff0000;`
- **Valores RGB**: `color: rgb(255, 0, 0);`

### Exemplo de Cores em CSS

```css
h1 {
    color: #4CAF50;
}

p {
    color: rgb(70, 130, 180);
}
```

---

## Espaçamento: Padding e Margin

O **`padding`** e o **`margin`** são usados para definir o espaçamento interno e externo dos elementos, respectivamente:

- **`padding`**: Espaçamento interno, entre o conteúdo e as bordas do elemento.
- **`margin`**: Espaçamento externo, entre o elemento e outros elementos ao seu redor.

### Exemplo de Padding e Margin

```css
div {
    padding: 20px;
    margin: 10px;
    background-color: #f4f4f4;
}
```
Neste exemplo, o conteúdo do **`<div>`** terá 20px de espaçamento interno e 10px de espaçamento externo em relação a outros elementos.


---

## Aplicando Bordas a Elementos

A propriedade **`border`** permite adicionar bordas aos elementos. Você pode personalizar a cor, estilo e espessura das bordas.

### Exemplo de Bordas em CSS

```css
div {
    border: 2px solid #4CAF50;
}
```

Aqui, uma borda sólida de 2px de espessura e cor verde será aplicada ao elemento **`<div>`**.


---

## Exercício Prático

1. Crie uma página HTML que inclua:
   - Um título (h1) e dois parágrafos (p).
   - Defina uma fonte personalizada para o título e outra fonte para os parágrafos.
   - Aplique cores diferentes ao título e ao parágrafo.
   - Adicione um espaçamento interno (padding) e externo (margin) a uma div.
   - Adicione uma borda à div.

---

### Estrutura Sugerida

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Estilos Básicos em CSS</title>
    <style>
        h1 {
            font-family: "Helvetica", sans-serif;
            color: #4CAF50;
        }

        p {
            font-family: "Arial", sans-serif;
            color: #333;
            text-align: justify;
        }

        div {
            padding: 20px;
            margin: 10px;
            border: 2px solid #4CAF50;
            background-color: #f4f4f4;
        }
    </style>
</head>
<body>
    <h1>Estilos Básicos para Textos e Elementos</h1>
    <p>Este é o primeiro parágrafo. Estamos aprendendo a aplicar estilos com CSS.</p>
    <p>Este é o segundo parágrafo, com uma fonte e cor diferentes.</p>

    <div>
        <p>Este parágrafo está dentro de uma div com padding, margin e uma borda aplicada.</p>
    </div>
</body>
</html>
```