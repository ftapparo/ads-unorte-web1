# Aula 9: IDs e Classes em CSS

## Introdução

Nesta aula, vamos aprender sobre o uso de **IDs** e **Classes** no CSS, que são usados para aplicar estilos específicos a elementos HTML. Você entenderá a diferença entre IDs e Classes, como usá-los corretamente e quando optar por um ou outro.

## O que são IDs e Classes?

- **Classes**: São usadas para aplicar o mesmo estilo a vários elementos. Um mesmo elemento pode ter várias classes.
- **IDs**: São usadas para identificar um único elemento em uma página. Cada elemento deve ter um ID exclusivo.

### Diferença entre ID e Classe:

- **Classe**: Definida com um ponto (`.`) no CSS. Pode ser reutilizada em vários elementos.
- **ID**: Definida com um cerquilha (`#`). Deve ser única para cada elemento em uma página.

### Exemplo de Classe

```html
<p class="destaque">Este parágrafo está em destaque.</p>
```

```css
.destaque {
    color: blue;
    font-weight: bold;
}
```

### Exemplo de ID

```html
<p id="importante">Este parágrafo é único e importante.</p>
```

```css
#importante {
    color: red;
    font-size: 20px;
}
```

---

## Quando Usar IDs e Classes?

- **Use Classes** quando você precisar aplicar o mesmo estilo a vários elementos. Classes são reutilizáveis e ideais para estilizar grupos de elementos.
  
- **Use IDs** quando você quiser estilizar apenas um elemento específico da página. IDs são exclusivos e devem ser usados apenas uma vez por página.

### Exemplo Prático de IDs e Classes

```html
<div class="caixa">
    <p class="texto">Este é um parágrafo dentro de uma caixa.</p>
</div>

<div id="caixa-unica">
    <p class="texto">Esta é uma caixa única com um ID exclusivo.</p>
</div>
```

```css
.caixa {
    background-color: #f4f4f4;
    padding: 20px;
    border: 1px solid #ccc;
}

#caixa-unica {
    background-color: #e0e0e0;
    padding: 30px;
    border: 2px solid #000;
}

.texto {
    font-family: Arial, sans-serif;
    color: #333;
}
```


---

## Como Utilizar Múltiplas Classes

Um elemento pode ter várias classes aplicadas a ele. Isso permite combinar estilos de diferentes classes de forma modular.

### Exemplo de Múltiplas Classes

```html
<p class="negrito destaque">Este texto está em negrito e em destaque.</p>
```

```css
.negrito {
    font-weight: bold;
}

.destaque {
    color: blue;
}
```

Nesse exemplo, o parágrafo tem tanto a classe **`negrito`** quanto a classe **`destaque`**, aplicando ambos os estilos.


---

## Especificidade no CSS

A especificidade define a prioridade dos seletores CSS. Se um elemento tiver estilos conflitantes, o navegador aplicará o estilo com a maior especificidade.

### Regras de Especificidade:

1. **ID**: Maior prioridade (seleciona um único elemento).
2. **Classe e atributos**: Média prioridade (pode ser aplicada a vários elementos).
3. **Elementos HTML**: Menor prioridade (como `p`, `h1`, etc.).

### Exemplo de Especificidade

```html
<p id="paragrafo-importante" class="destaque">Texto com ID e classe aplicados.</p>
```

```css
/* Estilo baseado no ID */
#paragrafo-importante {
    color: red;
}

/* Estilo baseado na classe */
.destaque {
    color: blue;
}
```

Neste exemplo, o ID tem maior especificidade, então o texto será exibido em vermelho, mesmo que a classe defina a cor azul.


---

## Exercício Prático

1. Crie uma página HTML que inclua:
   - Um parágrafo com um **ID** único.
   - Dois parágrafos com a mesma **classe**.
   - Aplique estilos diferentes para o ID e para a classe.

---

### Estrutura Sugerida

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Exemplo de IDs e Classes</title>
    <style>
        /* Estilo para o ID */
        #importante {
            color: red;
            font-size: 20px;
        }

        /* Estilo para a Classe */
        .destaque {
            color: blue;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <p id="importante">Este parágrafo tem um ID único.</p>
    <p class="destaque">Este parágrafo tem uma classe.</p>
    <p class="destaque">Este outro parágrafo também tem a mesma classe.</p>
</body>
</html>
```