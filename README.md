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

---
