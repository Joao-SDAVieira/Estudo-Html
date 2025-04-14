# Estudo-Html
Projetos e histórico de estudos de HTML e CSS.

# 📘 Estudos de CSS

Repositório dedicado ao estudo de **CSS** (Cascading Style Sheets), abordando desde os conceitos básicos até os seletores mais avançados e combinadores. Ideal para quem está começando ou quer revisar os fundamentos dessa poderosa linguagem de estilo.

---

## 📌 O que é CSS?

CSS (Cascading Style Sheets — Folhas de Estilo em Cascata) é uma **linguagem de estilos** usada para descrever a apresentação de documentos HTML. Ela **não é uma linguagem de marcação nem de programação**, e sim uma linguagem que define como os elementos HTML serão exibidos na tela, no papel ou em outros meios.

---

## 🎨 Formas de declarar CSS

### 1. CSS Inline
Estiliza diretamente na tag HTML usando o atributo `style`.

```html
<h1 style="background: red; color: white;">Título em CSS Inline</h1>
```

### 2. CSS Interno
Utiliza a tag `<style>` dentro da `<head>` do HTML.

```html
<head>
  <style>
    h1 {
      background: blue;
      color: white;
    }
  </style>
</head>
```

### 3. CSS Externo
Cria-se um arquivo `.css` separado e o vincula com a tag `<link>`.

**style.css**
```css
h1 {
  background: red;
  color: white;
}
```

**index.html**
```html
<head>
  <link rel="stylesheet" href="./assets/css/style.css">
</head>
```

> 📌 Observação: A ordem de prioridade é CSS inline > interno > externo.

---

## 🛠️ Ferramentas para Depuração

Todos os navegadores modernos possuem **DevTools**, que permitem:

- Inspecionar o HTML e CSS da página.
- Testar alterações diretamente no navegador.
- Simular diferentes tamanhos de tela (modo responsivo).

Use o atalho `F12` ou clique com o botão direito e escolha "Inspecionar".

---

## 🎯 Seletores CSS

Seletores definem **quais elementos HTML** receberão os estilos CSS.

### 🔹 Por Tag
```css
h1 {
  color: blue;
}
```

### 🔹 Por ID
```css
#titulo {
  background: lightblue;
}
```

### 🔹 Por Classe
```css
.titulo {
  color: brown;
}
```

Você pode combinar várias classes em um elemento:

```html
<p class="formatacao-padrao texto-maiusculas">Texto estilizado</p>
```

### 🔹 Universal
Aplica estilo a **todos os elementos** da página.

```css
* {
  font-style: italic;
}
```

### 🔹 Por Atributo
```css
[title] {
  background-color: blue;
}

[title="exemplo"] {
  background-color: red;
}
```

Outras variações:
- `[title~="termo"]`: Contém a palavra "termo"
- `[title|="prefixo"]`: Começa com "prefixo-"
- `[title^="inicio"]`: Começa com "inicio"
- `[title$="fim"]`: Termina com "fim"
- `[title*="parte"]`: Contém "parte"

---

## 🧩 Combinadores

### 🔹 Agrupamento
Aplica o mesmo estilo a múltiplos seletores:

```css
h1, p, .texto {
  color: red;
}
```

### 🔹 Combinador Descendente (espaço)
Seleciona elementos **dentro de outro**.

```css
div p {
  color: green;
}
```

### 🔹 Combinador Filho Direto (`>`)
Seleciona apenas **filhos diretos**:

```css
div > p {
  color: red;
}
```

### 🔹 Irmão Adjacente (`+`)
Seleciona o **primeiro irmão** que vem logo após:

```css
div + p {
  background: lightgreen;
}
```

### 🔹 Irmão Geral (`~`)
Seleciona **todos os irmãos seguintes**:

```css
h1 ~ p {
  color: blue;
}
```
## Propriedades de Dimensionamento e Espaçamento

As propriedades de dimensionamento e espaçamento em CSS permitem controlar o tamanho dos elementos e o espaço ao seu redor, proporcionando maior flexibilidade no layout da página.

### Largura e Altura

- **`width`**: Define a largura de um elemento.
- **`height`**: Define a altura de um elemento.

As unidades mais comuns são:

- **`px`**: Pixels (valor fixo).
- **`%`**: Porcentagem relativa ao elemento pai.
- **`em` / `rem`**: Relativas ao tamanho da fonte.
- **`vw` / `vh`**: Relativas à largura e altura da viewport.

Exemplo:

```css
div {
  width: 200px;
  height: 300px;
}
```

Valores especiais para `width` e `height`:

- **`auto`**: O navegador calcula automaticamente o tamanho.
- **`initial`**: Define o valor inicial da propriedade.
- **`inherit`**: Herdado do elemento pai.

Exemplo de uso do `inherit`:

```html
<style>
  #div-01 {
    background: lightblue;
    width: 200px;
    height: 300px;
  }
  #div-02 {
    background: lightgreen;
    height: inherit;
  }
</style>
<div id="div-01">
  Sou a div-01
  <div id="div-02">Eu sou a div-02</div>
</div>
```

### Altura e Largura Mínima e Máxima

- **`min-width` / `max-width`**: Define a largura mínima e máxima.
- **`min-height` / `max-height`**: Define a altura mínima e máxima.

Exemplo:

```css
button {
  background: pink;
  min-width: 200px;
  max-width: 200px;
  min-height: 200px;
  max-height: 200px;
}
```

### Margin

A propriedade `margin` define o espaçamento externo de um elemento.

- **`margin-top`**: Margem superior.
- **`margin-right`**: Margem à direita.
- **`margin-bottom`**: Margem inferior.
- **`margin-left`**: Margem à esquerda.

Shorthand para `margin`:

- **Um valor**: Aplica a todos os lados.
- **Dois valores**: Primeiro para cima/baixo, segundo para esquerda/direita.
- **Três valores**: Topo, laterais, inferior.
- **Quatro valores**: Topo, direita, inferior, esquerda (sentido horário).

Exemplo:

```css
#elemento-01 {
  background: orange;
  margin: 20px 20px 40px 5px;
}
```

Valores especiais:

- **`auto`**: O navegador calcula automaticamente a margem.
- **`inherit`**: Herdado do elemento pai.

*Nota*: É possível usar valores negativos para `margin`, o que pode resultar em sobreposição de elementos.

### Padding

A propriedade `padding` define o espaçamento interno de um elemento.

- **`padding-top`**: Preenchimento superior.
- **`padding-right`**: Preenchimento à direita.
- **`padding-bottom`**: Preenchimento inferior.
- **`padding-left`**: Preenchimento à esquerda.

Shorthand para `padding`:

- **Um valor**: Aplica a todos os lados.
- **Dois valores**: Primeiro para cima/baixo, segundo para esquerda/direita.
- **Três valores**: Topo, laterais, inferior.
- **Quatro valores**: Topo, direita, inferior, esquerda (sentido horário).

Exemplo:

```css
#elemento-01 {
  background: orange;
  padding: 20px 40px 50px 60px;
}
```

### Box Sizing

A propriedade `box-sizing` define como o tamanho total de um elemento é calculado.

- **`content-box`** (padrão): `width` e `height` se aplicam apenas ao conteúdo, excluindo `padding` e `border`.
- **`border-box`**: `width` e `height` incluem `padding` e `border`.

Exemplo:

```css
div {
  width: 200px;
  padding: 20px;
  border: 5px solid black;
  box-sizing: border-box;
}
```

Neste exemplo, o tamanho total do `div` será de 200px, incluindo o `padding` e a `border`.


## Cores
Existem diversas formas de definir a cor, elas são:

### Pré-definidas
Seleciona cores pelo nome, cores já definidas pelo CSS, é possível consultar exatamente a cor pelo w3schools.

```html
<style>
    #pre-definidas{
        color: purple
    }
</style>

<li id="pre-definidas">Cores pré-definidas</li>
```

Sendo possível colocar cores transparentes:

```html
<style>
    li{
        background: aquamarine
    }
    #current-color{
        background: transparent;
    }
</style>

<h1>Cores</h1>
<p>Existem várias formas de definirmos cores</p>
<ul>
    <li id="pre-definidas">Cores pré-definidas</li>
    <li id="current-color">Palavra-chave "current-color"</li>
</ul>
```

Para a cor de um outro atributo ter a mesma cor do atributo color:

```html
<style>
    #current-color{
        color: orange;
        border: 2px solid currentColor;
    }
</style>
```

Isso pode ser feito para `border`, `background`, entre outros.

### RGB e RGBA

```css
#rgb {
    color: rgb(70, 20, 80);
}

#rgba {
    color: rgba(255, 0, 0, 0.3);
}
```

### Hexadecimal

```css
#hex {
    color: #012ABC;
    color: #012ABC44; /* com transparência */
}
```

### HSL e HSLA

```css
#hsl {
    color: hsl(200, 100%, 50%);
    color: hsla(200, 100%, 50%, 0.3);
}
```

(hue de 0 a 360, saturation de 0 a 100%, lightness de 0 a 100%)

## Object-fit e Object-position
Usados para determinar o comportamento de dimensionamento de uma imagem dentro de um container.

### Object-fit
- `fill` (padrão)
- `contain`
- `cover`
- `none`
- `scale-down`

### Object-position
Controla a parte visível da imagem com `cover`, como `10px 10px`, `left top`, `center`, etc.

## Fundo de elementos
### Tipos
- `background-image: url()`
- `linear-gradient()`
- `radial-gradient()`
- `repeating-linear-gradient()`

### Camadas
```css
background-image: url('img1.jpg'), url('img2.jpg');
background-size: cover, contain;
```

### Redimensionamento com `background-size`
- `cover`
- `contain`
- `px` ou `%`
- Dois valores para altura e largura
- Camadas: `background-size: cover, contain;`

### Repetição com `background-repeat`
- `repeat-x`, `repeat-y`
- `space`, `round`, `no-repeat`
- Combinações: `repeat space`, `no-repeat round`

### Posição com `background-position`
- `bottom`, `top`, `left`, `right`, `center`
- `px`, `%`
- Combinação de dois valores

### Rolagem com `background-attachment`
- `fixed`
- `scroll`
- `local`

### Origem com `background-origin`
- `padding-box`
- `border-box`
- `content-box`

### Recorte com `background-clip`
- `padding-box`, `border-box`, `content-box`, `text`

### Atalho com `background`
```css
background: url('img.jpg') no-repeat center/cover;
```

## Bordas

### Tamanho com `border-width`
```css
border-width: 10px 20px 30px 40px;
```

### Estilo com `border-style`
- `none`
- `dashed`, `dotted`, `double`
- `groove`, `ridge`, `inset`, `outset`, `solid`

```css
border-style: dashed dotted solid double;
```

### Cor com `border-color`
```css
border-color: purple green yellow blue;
```

### Atalho com `border`
```css
border: 10px solid rgb(83, 8, 84);
```
## Arredondando Pontas com `border-radius`

A propriedade `border-radius` é utilizada para arredondar os cantos das bordas de um elemento.

### Sintaxe Básica

```css
border-radius: 10px;
```

Esse valor aplica um leve arredondamento a todos os cantos do elemento.

### Especificando Cada Canto

Você pode aplicar valores diferentes para cada canto, seguindo o sentido horário a partir do canto superior esquerdo:

```css
border-radius: 10px 20px 5px 8px;
```

- **10px**: canto superior esquerdo  
- **20px**: canto superior direito  
- **5px**: canto inferior direito  
- **8px**: canto inferior esquerdo  

### Efeito Oval

Para criar um efeito mais oval, utilize dois valores separados por uma barra:

```css
border-radius: 50px / 100px;
```

## Criando Círculos com `border-radius`

Se o elemento tiver a **mesma altura e largura**, você pode criar um círculo perfeito usando:

```css
border-radius: 50%;
```

Caso as dimensões sejam diferentes, o resultado será uma forma **oval**.

---

## Inserindo Imagens na Borda com `border-image-source`

A propriedade `border-image-source` permite inserir imagens ou gradientes nas bordas de um elemento. Para isso, deve-se também definir um `border` com estilo sólido e tamanho visível.

### Com Imagem

```css
border: 10px solid;
border-image-source: url('caminho/da/imagem.png');
```

Isso exibirá a imagem nas bordas do elemento.

### Com Gradiente

```css
border: 10px solid;
border-image-source: linear-gradient(red, blue);
```

Em vez de uma imagem, será exibido um **bloco em gradiente** nas bordas.

---

## Observação

Para que o `border-image-source` funcione corretamente, é essencial definir um `border-width` com valor maior que `1px`.

---
