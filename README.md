---
type: Page
title: CSS
description: null
icon: null
createdAt: '2025-02-06T18:40:04.775Z'
creationDate: 2025-02-06 15:40
modificationDate: 2025-06-06 15:58
tags: []
coverImage: null
---

Introduzindo CSS do básico ao avançado.

# O que é CSS

CSS é abreviação de Cascading Style Sheets ou FIlha de Estilo em Cascata.

É um mecanismo para adicionar estilos a um documento web HTML.

É uma linguagem de estilos, não é de marcação e nem de programação, apenas de estilos.

## Formas de declarar o CSS

Existem basicamente 3 formas de estilizar o HTML com css.

CSS inline - CSS inline é estilizar o html com o atributo "style" da tag, exemplo:

```html
<body>
    <h1 style="background: red; color: white">Dio - Digital Innovation One</h1>
    <h2 style="color: red;">
        Trilha de CSS 
    </h2>
</body>
```

CSS Interno - CSS interno é colocar o código css na head do código HTML utilizando seletores e a tag <style>. Por exemplo:

```html
    <title>Trilha de CSS</title>
    <style>
        h1{
            background: blue;
            color: white;
        }
        h2{
            color: blue
        }
    </style>
</head>
<body>
    <h1>Dio - Digital Innovation One</h1>
    <h2>
        Trilha de CSS 
    </h2>
```

OBS: O css inline é mais prioritário do que o interno, então o que for definido com o ATRIBUTO style será a forma final daquele estilo.

CSS Externo - CSS externo é feito criando um arquivo .css e esse aquivo é chamado na tag head da página.

EX:

É criado uma pasta chamada "assets", entro dela uma outra chamada "css" e dentro dessa pasta o arquivo "style.css"

No arquivo style.css:

```css
h1 {
    background: red;
    color: white;
}

h2{
    color: red;
}
```

No arquivo .html:

```html
    <title>Trilha de CSS</title>
    <link rel="stylesheet" href="./assests/css/style.css">

</head>
<body>
    <h1>Dio - Digital Innovation One</h1>
    <h2>
        Trilha de CSS 
    </h2>
    <h2>
        João 
    </h2>
</body>
```

É utilizada a tag <link> para referenciar o arquivo .css.

## Depurando o CSS

Todos os navegadores possuem uma ferramenta chamada dev tools, utilizada para depurar o código css.

Para isso é utilizado a parte de inspecionar do chrome por exemplo.

Nele é encontrado o html da página junto ao css, sendo possível fazer testes e outras coisas apenas com o navegador.

A aba principal é a elements e styles para o css

Também é possível ver a página em telas diferentes



# Seletores

Seletores nada mais é do que a forma que será determinada a formatação do css. Se será por tag, por id, por classe,etc.



## Tipos de seletores

### Seletor por tag

O seletor por tag é você determinar que toda marcação que tiver uma tag específica terá determinado comportamento, exemplo:

```html
    <style>
        h1{
            background-color: lightblue;
            color: darkblue;
        }
        div{
            background: blue;
            color: yellow;
        }
    </style>
```

Assim é determinado que toda tag div ou h1 da página terão essas características específicas que o css determinou.

### Seletores de id

Aplica o estilo através do id da tag, exemplo 

```html
        #texto-boas-vindas {
            background-color: blue;
        }
        #explicacao-seletores {
            background-color: aqua;
        }
    </style>
</head>
<body>
    <h1>Seletores CSS</h1>
    <p id="texto-boas-vindas">Bem vindo</p>
    <p id="explicacao-seletores">No css possuímos seletores por ID</p>
```

Nesse caso cada tag p com um id específico terá o seu estilo.



### Seletor de classe

O seletor de classe é utilizado quando você quer padronizar alguns estilos na página, assim sendo definida uma classe que as tags que for dessa classe terá o estilo passado. Para definir o estilo é usado um . ou invés do # do seletor de id. Exemplo:

```html
    <style>
        .formatacao-padrao{
            color: brown;
        }
    </style>
</head>
<body>
    <h1>Seletores CSS</h1>
    <p class="formatacao-padrao">Bem vindo</p>
    <p class="formatacao-padrao">No css possuímos seletores por ID</p>
```

Também é possível passar duas classes com um espaço entre as duas classes, exemplo:

```html
    <style>
        .formatacao-padrao{
            color: brown;
        }
        .texto-maiusculas{
            text-transform: uppercase;
        }
    </style>
</head>
<body>
    <h1>Seletores CSS</h1>
    <p class="formatacao-padrao">Bem vindo</p>
    <p class="formatacao-padrao texto-maiusculas">No css possuímos seletores por ID</p>
```



### Seletores universais

Seletores universais determina o estilo de toda a página em questão independente da tag. Para isso é utilizado apenas um *:

```html

        *{
            font-style: italic;
        }
    </style>
</head>
<body>
    <h1>Seletores CSS</h1>
    <p class="formatacao-padrao">Bem vindo</p>
    <p class="formatacao-padrao texto-maiusculas">No css possuímos seletores por ID</p>
</body>
</html>
```

Para deixar todas as tags em italico. Isso é usado também para padronizar a fonte.

### Seletor de atributos

Como o nome diz, vai fazer a formatação pelo atributo da tag. Nele é utilizado colchetes [] envolta do atributo

```html
<style>
        [title]{
            background-color: blue;
        }
    </style>
</head>
<body>
    <h1>Seletores CSS</h1>
    <p title="texto">Bem vindo</p>
    <p title="texto">No css possuímos seletores por ID</p>
```

Mas também é possível indicar um atributo e valor específico usando o valor de igual =:

```html
<style>
        [title="texto-tipo1"]{
            background-color: blue;
        }
    </style>
</head>
<body>
    <h1>Seletores CSS</h1>
    <p title="texto-tipo1">Bem vindo</p>
    <p title="texto-tipo2">No css possuímos seletores por ID</p>
```

Assim apenas os atributos específicos com titulo "texto-tipo1" terão a formatação.

Outra forma também é usar um ~ para indicar que basta o valor ter o termo expecífico, exemplo:

```html
<style>
        [title~="texto"]{
            background-color: blue;
        }
    </style>
</head>
<body>
    <h1>Seletores CSS</h1>
    <p title="texto tipo1">Bem vindo</p>
    <p title="texto tipo2">No css possuímos seletores por ID</p>
```

Desta outra forma todos que possuem "texto" como valor do atributo title terão esse estilo.

Também pode-se fazer a mesma coisa mas esperando um hífen "-" no valor do atributo através do "|":

```html
    <style>
        [title|="texto"]{
            background-color: blue;
        }
    </style>
</head>
<body>
    <h1>Seletores CSS</h1>
    <p title="texto-tipo1">Bem vindo</p>
    <p title="texto-tipo2">No css possuímos seletores por ID</p>
    <p title="texto tipo1">Bem</p>
    <p title="texto tipo2">No css possuímos</p>
```

Assim basta ter o valor "texto" e um hífen para ser aplicado o estilo.

Também é possível achar o valor do atributo pelo sulfixo e prefixo, com:

^ - antes do igual = para o prefixo

$ - antes do igual = para o prefixo

Ou até mesmo um valor específico em qualquer parte do atributo, com um * antes do igual = .



## Combinadores

### Agrupamento de seletores

Até então, supondo que tenhamos um código que possuem tags diferentes que precisam ser estilizadas, seria necessário clocar um identificador em cada uma das tags ou passar o estilo de cada uma das tags.

Com agrupamento de seletores, é possível passar por vírgulas várias tags diferentes a estilizar:

```html
    <style>
        h1, p, div{
            color: red
        }

    </style>
</head>
<body>
    <h1>Agrupamento de Seletores</h1>
    <p>Podemos aplicar as mesmas regras CSS para várias</p>
    <div>Assim, Não precisamos ficar copiando e colando código</div>
    <br><br>
    <a id="link-referencia" href="#">Clique aqui para ver exemplos</a>
    
    <br><br>
    <a id="link-suporte" href="#">Clique aqui para entrar em contato com o suporte</a>
    <br><br>
    <a id="botao-voltar" href="#">Voltar</a>
    <br><br>
    <button id="botao-fechar">fechar página</button>

</body>
```

Também é possível mesclar com classes e atributos da seguinte forma:

```html
 <style>
        .texto, h1, #link-referencia{
            color: red;
        }
    </style>
</head>
<body>
    <h1>Agrupamento de Seletores</h1>
    <p class="texto">Podemos aplicar as mesmas regras CSS para várias</p>
    <div class="texto">Assim, Não precisamos ficar copiando e colando código</div>
    <br><br>
    <a id="link-referencia" href="#">Clique aqui para ver exemplos</a>
    
    <br><br>
    <a id="link-suporte" href="#">Clique aqui para entrar em contato com o suporte</a>
    <br><br>
```

Ou até mesmo pelo id misturado com o estilo que já foi aplicado, por exemplo:

```html
<meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trilha de CSS</title>
    <style>
        .texto, h1, #link-referencia{
            color: red;
        }
        h1, [id^="botao"]{
            background: blue;
        }
    </style>
</head>
<body>
    <h1>Agrupamento de Seletores</h1>
    <p class="texto">Podemos aplicar as mesmas regras CSS para várias</p>
    <div class="texto">Assim, Não precisamos ficar copiando e colando código</div>
    <br><br>
    <a id="link-referencia" href="#">Clique aqui para ver exemplos</a>
    
    <br><br>
    <a id="link-suporte" href="#">Clique aqui para entrar em contato com o suporte</a>
    <br><br>
    <a id="botao-voltar" href="#">Voltar</a>
    <br><br>
    <button id="botao-fechar">fechar página</button>
```

Essa abordagem possui implicitamente um "ou" para selecionar o elemento que vai sofrer a ação, isso porque se não tivermos nenhuma tag "h1" por exemplo, a estilização será feita apenas na outra seleção que foi passada.

Já para agrupar e selecionar apenas com identificadores específicos, é utilizado um . entre as especificações, por exemplo:

```html
<style>
        p.texto{
            color: red;
        }
    </style>
</head>
<body>
    <h1>Agrupamento de Seletores</h1>
    <p class="texto">Podemos aplicar as mesmas regras CSS para várias</p>
    <p class="teste">Teste</p>
    <div class="texto">Assim, Não precisamos ficar copiando e colando código</div>
    <br><br>
```

Apenas os elementos que tem a tag p e o atributo texto terão a estilização, os demais não.

Ou por exemplo um elemento que deve possuir duas classes específicas:

```html
 <style>
        .texto.teste{
            color: red;
        }
    </style>
</head>
<body>
    <h1>Agrupamento de Seletores</h1>
    <p class="texto">Podemos aplicar as mesmas regras CSS para várias</p>
    <p class="teste texto">Teste</p>
    <div class="texto">Assim, Não precisamos ficar copiando e colando código</div>
    <br><br>
```



### Combinador descendente (espaço)

Os combinadores descendente servem para determinar um elemento dentro do outro que terá um estilo, em ordem descendente, eles são separados por espaço, por exemplo:



```html
<style>
        li {
            color: blue;
        }
        li li{
            color:green
        }
        #lista-01 li{
            background: lightblue;
        }
    </style>
</head>
<body>
    <ul>
        <li class="fundo-verde" id="lista-01">
            <div>Item 1</div>
            <ul id="sublista - 01">
                <li>Subitem A</li>
                <li>Subitem B</li>
            </ul>
        </li>
        <li class="fundo-verde" id="lista-02">
            <div>Item 2</div>
            <ul id="sublista - 02">
                <li>Subitem A</li>
                <li>Subitem B</li>
            </ul>
        </li>
        <li class="fundo-azul" id="lista-03">
            <div>Item 3</div>
            <ul id="sublista - 03">
                <li>Subitem A</li>
                <li>Subitem B</li>
            </ul>
        </li>
    </ul>
```

Todos os li primeiro terão a cor blue, depois os li que estão dentro de outro li serão green.

O mesmo se faz com id, no caso, apenas o li que estão dentro do elemento com o id "lista-01" será lightblue.

O mesmo pode-se fazer com classe, inclusive alternando entre tag, classe, id, etc:

```html
<style>
        .fundo-verde li{
            background: lightgreen;
        }
        .fundo-azul li{
            background: lightblue;
        }
        li {
            color: red
        }
        .fundo-verde #sublista-01 li{
            color: black
        } 

    </style>
</head>
<body>
    <ul>
        <li class="fundo-verde" id="lista-01">
            <div>Item 1</div>
            <ul id="sublista-01">
                <li>Subitem A</li>
                <li>Subitem B</li>
            </ul>
        </li>
        <li class="fundo-verde" id="lista-02">
            <div>Item 2</div>
            <ul id="sublista-02">
                <li>Subitem A</li>
                <li>Subitem B</li>
            </ul>
        </li>
        <li class="fundo-azul" id="lista-03">
            <div>Item 3</div>
            <ul id="sublista-03">
                <li>Subitem A</li>
                <li>Subitem B</li>
            </ul>
```

### Combinador filho (>)

Esse combinador é separado pelo simbolo de maior >.

Ele serve para passar o estilo para um elemento que é filho direto de outro (que está diretamente na hierarquia), exemplo:

```html
<style>
        div p {
            background: lightgreen;
        }

        div > p{
            color: red
        }
    </style>
</head>
<body>
    <div>
        <p>Parágrafo 1 dentro da div</p>
        <p>Parágrafo 2 dentro da div</p>
        <span>
            <p>Parágrafo 3 dentro da div, dentro do span</p>
        </span>
    </div>
    <p>Parágrafo 4 fora da div</p>
    <p>Parágrafo 5 fora da div</p>
```

No primeiro seletor é utilizado o combinador descendente, porém as vezes queremos só aplicar uma modificação ao filho direto da div, o filho da tag span que está dentro dessa div não deve sofrer modificação.

então usa-se div>p, ou seja, apenas os p que estão dentro de div terão o estilo.



### Combinador irmão adjacente (+)

Esse combinador faz a estilização apenas para o primeiro elemento identificado com o mesmo nivel de hierarquia, exemplo:



```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trilha de CSS</title>
    <style>
        div + p{
            color: tomato;
        }
        .fundo-verde + p{
            background: lightgreen;
        }
    </style>
</head>
<body>
    <div class="fundo-verde">
        <p>Parágrafo 1 dentro da div</p>
        <p>Parágrafo 2 dentro da div</p>
        <span>
            <p>Parágrafo 3 dentro da div, dentro do span</p>
        </span>
    </div>
    <p>Parágrafo 4 fora da div</p>
    <p>Parágrafo 5 fora da div</p>

    <div class="fundo-verde">
        <p>Parágrafo 6 dentro da div</p>
        <p>Parágrafo 7 dentro da div</p>
        <span>
            <p>Parágrafo 8 dentro da div, dentro do span</p>
        </span>
    </div>
    <p>Parágrafo 9 fora da div</p>
    <p>Parágrafo 10 fora da div</p>

    <div class="fundo-azul">
        <p>Parágrafo 11 dentro da div</p>
        <p>Parágrafo 12 dentro da div</p>
        <span>
            <p>Parágrafo 13 dentro da div, dentro do span</p>
        </span>
    </div>
    <p>Parágrafo 14 fora da div</p>
    <p>Parágrafo 15 fora da div</p>
</body>
```

Assim, para o color:tomato apenas os elementos com a tag p que tem o valor:

Parágrafo 4 fora da div, Parágrafo 9 fora da div e Parágrafo 14 fora da div

Será aplicado esse estilo, já o background: lightgreen será para o:

Parágrafo 4 fora da div e Parágrafo 9 fora da div

Isso porque essas tag p estão no mesmo nivel de hierarquia que a sua div anterior

### Combinador irmão em geral (~)

Semelhante ao anterior, mas nesse caso aplica para todos os irmãos, não apenas para os que estão logo em seguida:

```html
<style>
        div ~ p{
            color: tomato;
        }
        .fundo-verde + p{
            background: lightgreen;
        }
    </style>
```

## Propriedades de Dimensionamento e Espaçamento

Existem diversas propriedades para dimensionamento e espaçamento, elas são utilizadas para modelar o tamanho dos elementos da página, tendo assim mais controle do que acontece.

### Largura e altura

Para dimensionar a largura, usa-se o width no css.

Deve ser passada a quantidade, por exemplo 200, junto a unidade de medida.

Sobre as unidades de medidas existem diversas, porém nesse primeiro momento é utilizado apenas px (pixels).

Já para dimensionar a altura é usado height, da mesma maneira do px.

Outras formas de declarar a largura por exemplo, é no width utilizar "auto", que de acordo com a tag, o elemento terá uma largura padrão do css

Também pode ser utilizado o initial que também pega um valor padrão do css.

Além desses, temos a palavra reservada inherit, que serve para o elemento filho herdar o atributo css da tag pai, exemplo:

```html
    <style>
        #div-01{
            background: lightblue;
            width: 200px;
            height: 300px
        }
        #div-02{
            background: lightgreen;
            height: inherit;
        }

    </style>
</head>
<body>
    <div id="div-01">
        sou a div-01
        <div id="div-02">Eu sou a div 02</div>
    </div>
```

A tag filha terá o mesmo tamanho da tag pai.

### Altura e largura mínima e máxima

Para elementos como botão que tem sua altura e largura responsivas de acordo com o texto, é interessante definir um range de tamanho dele. Para isso pode ser utilizado:

min-width e max-width: para largura máx e min

min-height e max-height: para altura máx e min

```html
button{
            background: pink;
            min-width: 200px;
            max-width: 200px;
            min-height: 200px;
            max-height: 200px;
        }
    </style>
</head>
<body>
    <button>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Cum praesentium quia magnam incidunt iure, dolores animi placeat enim aspernatur magni totam dicta voluptatibus illo architecto facere ad rerum, veritatis blanditiis! Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur rerum illum nobis reprehenderit quasi velit dolorum quo quas aperiam aliquid, magni quidem dolorem architecto earum! Voluptas quas necessitatibus repudiandae porro.
    </button>
```

### Margin

É possível definir as dimensões da margin, que é basicamente o lado de fora da borda do elemento.

Para a margin temos algumas propriedades, como:

margin-bottom: a margin embaixo

margin-top: a margin em cima

margin-left: a margin da esquerda

margin-right: a margin da direita

```html
<style>
        div{
            width: 300px;
            height: 300px;
        }
        #elemento-01{
            background: orange;
            margin-bottom: 50px;
        }
        #elemento-02{
            background: purple;
            margin-top: 10px;
            margin-left: 25px;
            margin-right: 30px;
        }
    </style>
</head>
<body>
    <div id="elemento-01"></div>
    <div id="elemento-02"></div>
</body>
```



Além disso é possível definir uma margem geral, para não precisar ficar definindo cada margin.

para isso pode-se passar até 4 valores para a propriedade "margin", dependendo da quantidade de valores que for passado terá um comportamento diferente, sendo:

Um valor - Esse valor para todos os lados do elemento

dois valores - O primeiro valor em cima e embaixo, o segundo valor para as laterais

três valores - O primeiro em cima, o segundo dos lados, o terceiro embaixo

quatro valores - Cada um para um lado no sentido horário, em cima, direita, baixo e esquerda.

```html
#elemento-01{
            background: orange;
            margin: 20px 20px 40px 5px;
        }
```

O margin também possui inherit e auto.

auto- faz com que o elemento fique centralizado na tela

Um detalhe sobre o margin também é que é possível usar valores negativos. Isso serve para esconder parte do elemento fora da tela por algum motivo.

### Padding

A padding é parecida com a margin, a diferença é que a padding é dentro da borda, então é uma camada interna do elemento.

```html
    <style>
        div{
            width: 200px;
            color: white;
        }
        #elemento-01{
            background: orange;
            padding: 20px 40px 50px 60px
            
        }
        #elemento-02{
            background: purple;

        }
    </style>
</head>
<body>
    <div id="elemento-01">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla, dignissimos itaque. Voluptate, officiis dicta totam animi debitis fugit, voluptates saepe libero harum porro vero impedit aspernatur delectus sint incidunt molestias?</div>
    <div id="elemento-02">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Iure, doloremque! Voluptatum et nobis quaerat vel autem recusandae ex a tenetur pariatur ullam fuga, voluptatibus perspiciatis doloremque repellendus error eum tempora!</div>
</body>
```

O funcionamento é exatamente o mesmo de margin

### Box sizing

A propriedade box sizing, basicamente vai definir se vão ser respeitadas largura e altura definidas para o elemento.

border-box - repeita o tamanho definido

content-box - vai de acordo com o que for passado

Isso porque muitas vezes, quando for feito uma definição de margin e padding, o tamanho do elemento ultrapassa o tamanho já definido para o elemento.

Assim é reduzido ou aumentado o tamanho do conteúdo interno do elemento.

## Cores

Existem diversas formas de definir a cor, elas são:

### Pré definida

pre-definidas - seleciona cores pelo nome, cores já definidas pelo css, é possível consultar exatamente a cor pelo w3schools

```html
    <style>
        #pre-definidas{
            color: purple
        }
    </style>

    <li id="pre-definidas">Cores pré-definidas</li>
```

Sendo possível colocar cores transparentes

```html
<style>
        li{
            background: aquamarine
        }
        #current-color{
            background: transparent;
        }
    </style>
</head>
<body>
    <h1>Cores</h1>
    <p>Existem várias formas de definirmos cores</p>
    <ul>
        <li id="pre-definidas">Cores pré-definidas</li>
        <li id="current-color">Palara-chave "current-color"</li>
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

Isso podendo ser feito para a border, backgoud, entre outros valores da tag:

### RGB

Os valores de cor com rgb são passados por uma função chamada rgb() que recebe de 0 a 255 quanto terá para vermelho, verde e azul

rgb(red, green, blue)

por exemplo:

```html

        #rgb{
            color: rgb(70, 20, 80)
        }
```

também pode ser considerado a opacidade/transparencia com o rgba, usando a escala de 0.0 até 1.0, onde 1.0 é totalmente preenchido e não transparente e 0.0 é totalmente transparente:

```html
        #rgba{
            color: rgba(255, 0, 0, 0.3)
        }
```

Podendo também omitir o 0 e pasar apenas .3 por exemplo.

### Hexadecimal

É possível utilizar tbm a escala de cores de hexadecimal, indo de 0 até F. Onde 000000 é preto e FFFFFF é branco.

```html
        #hex{
            color: #012ABC
        }
```

Azul

Podendo passar dois valores a mais para a transparencia (o padrão são 6, os dois a mais são a transparencia):
​

        #hex{

            color: #012ABC44

        }

```html
        #hsl{
            color: hsl(hue, saturation, lightness);
        }
```

hue é o grau da roda de cores (0 a 360 graus)

0 e 360 é vermelho

120 é verde

240 é azul 

Saturation é valor percentual de 0 a 100%

0 é um tom de cinza

100% é a cor total

lightness é a luminosidade da cor

0% é preto

100% é branco

```html
        #hsl{
            color: hsl(200, 100%, 50%);
        }
```

Aqui temos um azul claro

Também é possivel usar hsla para a transparencia:

```html
     #hsl{
            color: hsla(200, 100%, 50%, 0.3);
        }
```



## Object-fit e Object-position

ambos são utilizados para determinar o comportamento de dimensionamento de uma imagem que fica dentro de um container (elemento pai)

### Object-fit

é como a imagem vai preencher o container que ela está, por exemplo uma div, tendo diversos valores possíveis definidos no css, como:

fill: O padrão, preenche todo o elemento mas destorcendo a imagem

contain: imagem sem destorcer mas tentando pegar um bom espaço do elemento.

cover: Imagem maior, preenchendo o container mas sem distorcer a imagem, mas cortando uma parte dela.

none: Fica gigante

scale-down = encaixa da melhor maneira possível

### Object-position

 É utilizado principalmente com o object-fit cover, ele vai determinar qual parte da imagem vai preencher o container, ele pode receber:

valor do eixo horizontal e vertical separados por espaço, ex: object-position: 10px 10px

isso em px ou em %, onde 50% é o padrão.

Também é possível utilizar comandos especificos como:

object-position: left 50%

right

center

right 

right top (para ver em cima)

right center (ver centralizado)

right bottom (embaixo)

right start ou end

## Fundo de elementos

É possível colocar uma imagem utilizando a propriedade backgound-image: url()

linear-gradient(cor_inicial, cor_final, uma outra cor final) para fazer um gradiente de cores na imagem

radial-gradient() um gradiente de dentro para fora

repeating-linear-gradient() é um gradient que vai se repetir e ter uma ordem de listras:

repeating-linear-gradient(to top, blue 0 20 px, lightpink 20px 40 )



esse site possui esses estilos de backgound:

[CSS3 Patterns Gallery](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/01a63367-d8a3-486c-9b0f-1730ab0bd860)


É possível criar camadas passando o backgound-image, passando mais de uma url() separado por virgula para essa propriedade

### Redimensionando imagens de fundo dos elementos

backgound-size determina diversos comportamentos da imagem de backgound, sendo:

backgound-size: cover - nesse caso a imagem cobre todo o elemento, porém muitas vezes não pegando a imagem por completo;

backgound-size: contain - a imagem aparece por completo no elemento, mas a imagem se repete no espaço vazio do elemento por ser um comportamento padrão;

backgound-size: 50% ou em px - passa o tamanho que a imagem vai ocupar (largura)

backgound-size: px/% e px/% - passando dois valores, um para altura e outro para largura

backgound-size com camadas de imagens - passando duas imagens no backgound image (camadas) é possível passar todos os valores citados anteriormente mas separando por virgula a formatação aplicará para a respectiva imagem da camada.

ex:

backgound-size: cover, contain - a primeira imagem terá o comportamento de cover e a segunda de contain

### Repetição das imagens de fundo

O comportamento padrão do css é fazer com que a backgound image se repita até preencher o elemento.

backgound-repeat: repeat-x - só se repetirá horizontalmente, o resto do elemento ficara vazio

backgound-repeat: repeat-y - só se repetirá verticalmente, o resto do elemento ficara vazio

backgound-repeat: space - aplica um espaço entre a repetição das imagens (com imagens completas

backgound-repeat: round - ajusta a repetição para as imagens repetidas preencherem todo o elemento de forma que o tamanho de todas fiquem iguais, encaixando todas no elemento

backgound-repeat: no-reapeat - para a imagem ser exibida apenas uma vez

Para passar o comportamento vertical e horizontal, basta passar os valores separados por espaço, ex:

backgound-repeat: repeat space (assim a imagem vai se repetir, mas o space só terá no eixo vertical y)

backgound-repeat: no-repeat round (não se repete horizontalmente x e deixa a repetição ajustada para preenchimento no y

### Posicionamento da imagem de fundo

efeito paralax

Definindo o background-repeat: no-repeat é possível posicionar a imagem de fundo.

backgound-position: bottom ou top, left ou right

Também podendo passar em pixels (px)

ex: 200 px ou 10 px.

Ou porcentagem como 5% ou 20%

Pode-se passar mais de um valor, para eixo vertical e horizontal.

ex: backgound-position: center top (eixo horizontal fica centralizado mas no vertical fica no topo)

### Propriedade background-attachment

Essa propriedade serve para gerar efeito de a imagem da caixa manter fixa ou flexivel conforme o usuário rola a página.

background-attachment: fixed (a imagem vai ficar fixa, não vai descer junto com o elemento que a imagem está ou a página geral, gerando um efeito 3d)

background-attachment: scroll (quando rolar o conteudo do elemento ele fica parado mas com a página ele acompanha)

background-attachment: local (sem efeito acompanha a página normal)

### Propriedade backgound-origin

backgound-origin: padding-box (imagem não oculpa a borda mas ocupa todo o padding)

backgound-origin: border-box (a imagem cobre também a borda)

backgound-origin: content-box (cobre apenas a área de conteúdo do elemento)

### Propriedade backgound-clip

Parecido com a origin

backgound-clip: padding-box (igual o origin)

backgound-clip: border-box (igual o origin)

backgound-clip: content-box (igual o origin)

backgound-clip: text (aplica o backgound-image em um texto

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/cfb16238-e391-429c-ad60-4fc93722dd6f)

### Propriedade backgound

A propriedade background consegue receber todas as outras propriedades, basta passar o valor dela. Como se fosse um coringa

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/ec24c4cf-7a80-4583-9b6e-6278b20651ea)

## Bordas

### Tamanho da borda

border-width: 10px; - define o tamanho da borda (expessura)

é possível aplicar o valor da borda especificamente para a vertical e para horizontal:

border-width: 10px 20px (10 em cima e embaixo, 20 na esquerda e dir)

border-width: 10px 20px 30 px (10 topo, 20 laterais, 30 embaixo)

border-width: 10px 20px 30 px 40 px (para cada um em sentido horário a partir de cima)

```html
  .exemplo{
            background-color: palevioletred;
            width: 200px;
            height: 200px;
            border-style: solid;
            border-width: 10px 20px 30px 40px;
        }
```

### Estilo de borda

border-style: 

o valor padrão é none.

border-style: dashed (forma vários traços na borda)

border-style: dotted (forma vários pontos na borda)

border-style: double (cria duas linhas nas duas extremidades da borda):

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/ad2d1375-f9eb-41c8-ab5d-210a90b68d56)

border-style: groove (da um efeito 3d a borda, lembrando botão pressionado)

border-style: ridge (efeito de botão elevado)

border-style: inset (botão afundado)

border-style: outset (impressão de botão saindo da tela)

border-style: solid (borda preenchida, completa)

é possível misturar esses estilos assim como o width:

border-style: dashed dotted solid double

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/9bb1d596-16e6-4041-bfc0-01fc2abb2eca)

### Cor da borda

Por padrão a borda tem a cor do elemento (propriedade color)

Para alterar especificamente a borda usa-se o border-color

Ela possui as cores rgb, hexadecimais, etc.

border-color: purple

pode-se passar vários valores para cada parte da borda:

border-color: purple green yellow blue

### Propriedade border

Pode-se passar todas as propriedades em uma só, a border:
border: 10px solid rgb(83, 8, 84)

para definir as caracteristicas gerais da borda, para passar cada lado basta user border-bottom, border-top, border-left, border-right.

### Arredondando as pontas/cantos com border-radius

O atributo border-radius serve para arredondar as pontas das bordas.

border-radius: 10px;

deixa os cantos levemente arredondados

pode-se passar alguns outros tamanhos para selecionar quais pontas terão quais arredondamentos como:

border-radius: 10px 20px 5px 8px (topo esquerdo e sentido horário)

pode-se passar da seguinte maneira para ter um comportamento mais oval:

border-radius: 50px/100px

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/0affd703-b6b3-458e-8ee7-e27af24c9010)

Fazendo circulo:

Tendo a mesma altura e largura para o elemento, é possível fazer um circulo perfeito passando:

border-radius: 50%

caso tenha dimensões diferentes para o elemento ele ficará oval

### Propriedade border-image-source

Para colocar imagem na borda se utiliza border-image-source juntamente com border: solid (e algum tamanho maior que 1px para ficar visivel)

border-image-source: url('') vai ficar a imagem nas pontas

ou

border-image-source: linear-gradient(red, blue)

Para invés da imagem, ter um bloco em gradient

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/5f6709e1-99ac-4f52-bbb3-f09f559073ed)

### Propriedade border-image-slice

essa propriedade serve para formatar uma divisão da imagem e colocar na borda, a imagem é divida em 9 pontos e é colocada de forma diluida na borda do elemento, é importante utilizar essa propriedade com border-image-repeat: repeat.



### border-image-repeat

Determina como vai funcionar a repetição da imagem na borda, por exemplo:

border-image-repeat: round - vai fazer com que a repetição fique ajustada na borda, sem cortes.

border-image-repeat: space - dependendo do tamanho do elemento, o space vai fazer com que a imagem se ajuste na borda com um espaço.

Da mesma forma que as demais propriedades é possível determinar o comportamento da propriedade para o eixo vertical e horizontal passando eles atraves de espaço entre eles.



### border-image-outset

Essa propriedade vai determinar em px a distancia entre a borda e a imagem. podendo ser passado valores para cada lado do elemento ou eixos combinados.



### Utilizando todas as propriedades com a propriedade border-image

A propriedade border-image pode ser utilizada para combinar as propriedades anteriores. para isso:

"border-image: {url(url da imagem)} {o slice} {repeat}"

ex: border-image: url("../image/imagem.png") 169 round

Para colocar outras propriedades

largura do elemento:

"border-image: {url(url da imagem)} {o slice} / {qtd pixels} {repeat}"

ex: border-image: url("../image/imagem.png") 169 / 10px round

para o outset:

ex: border-image: url("../image/imagem.png") 169/ 10px / 1 round

## Fontes

É possível personalizar a fonte do texto da página através do CSS com propriedades como font-family.

Também é possível importar fonts que não possui de forma padrão no computador do usuário ou do desenvolvedor através de ferramentas como google fonts.

Para personalizar uma font com as fontes padrões, basta utilizar o font-family, é possível passar a font e as fonts alternativas caso a principal não tenha no navegador do usuário:

```css
* {
    font-family: "Timess Neew Rooooman", "Ariaal", fantasy;
}
```

No caso times new roman e arial estão escrito errado (ou seja, o navegador não encontrará a fonte) então é utilizado pelo navegador a font fantasy.

obs: fontes com mais de um nome separado por espaço deve ter aspas.

### Colocando fontes externas com @font-face

Até o momento, fontes como "Roboto" não são disponíveis por padrão, então é necessário adquirir ela de forma externa, ou seja, o código a seguir não funcionrá:

```css
* {
    font-family: Roboto;
}
```

Então, uma vez que foi instalado o pacote de fonts no computador, basta utilizar:

```css
@font-face{
    font-family: Roboto;
    src: local(),url("../fonts/Roboto-Bold.ttf")
}

p {
    font-family: Roboto;
  }
```

font-family determina o nome que você vai dar para a font, src é o local onde está o arquivo .ttf.

Além disso é possível determinar mais de uma fonte dependendo do comportamento da font, por exemplo, determinar uma font diferente para o font-weight normal e bold:

```css
@font-face{
    font-family: Roboto;
    src: local(),url("../fonts/Roboto-Regular.ttf");
    font-weight: normal;
}

@font-face{
    font-family: Roboto;
    src: local(),url("../fonts/Roboto-Bold.ttf");
    font-weight: bold;
}

p {
    font-family: Roboto;
    font-weight: normal;
}

h1{
    font-family: Roboto;
    font-weight: bold;
}
```

### Fontes externas com @import()

Para importar as fontes externas de forma menos complexas, pode-se utilizar o import(), que dispensa a necessidade de baixar arquivos externos, basta copiar a url do google por exemplo onde fica a fonte desejada:

```css
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100..900;1,100..900&display=swap');

* {
    font-family: Roboto;
}
```

### Alterando o tamanho da fonte com font-size

com a propriedade font-size é possível determinar o tamanho da fonte em px ou passar alguns valores padrões, do menor para o maior:

font-size: xx-small

font-size: x-small

font-size: small

font-size: medium

font-size: large

font-size: x-large

font-size: xx-large

Também é possível determinar se o font-size do elemento filho vai ser menor ou maior do que o tamanho já determinado para o elemento pai, ex:

```css
div p {
  font-size: smaller
}
```

a fonte do elemento p que é filho de div será menor que o div.

### Estilo de fonte font-style

É possível determinar o estilo da fonte com font-style, deixando o estilo da fonte como italic ou oblique por exemplo

```css
p {
  font-style: oblique
}
```

### Espessura das fontes com font-weight

Com a propriedade font-weight é possível determinar a espessura das fontes, a estilização da espessura que você determina no css será buscada diretamente nas configurações da fonte que está sendo utilizada, então é possível que alguma espessura (muito alta ou muito baixa) não seja possível:
​

```css
p{
  font-weight: 200px
}
```

Existem algumas palavras específicas, como:

font-weight: normal

font-weight: bold

font-weight: lighter (menos espessa que o elemento pai)

font-weight: bolder (mais espessa do que o elemento pai)

### Espaçamento com font-strecht

Uma propriedade que nem sempre possui suporte mas pode ser muito útil é o font-strecht para aumentar o espaçamento do texto.

### Espaçamento entre linhas com line-height

É possível determinar o espaçamento das linhas, por padrão é utilizado o tamanho da font, mas também é possível personalizar, passando valores em porcentagem, px, ou valores que se referem a quantidade de vezes em relação ao tamanho da font:
​

```css
p {
  line-height: 2;
}
```

espaçamento duas vezes o tamanho da fonte.

### Propriedade resumida font

```css
p {
  font: 20px Arial, sans-serif;
}
```

Consegue definir a fonte principal, secundária e o tamanho apenas com uma propriedade

Também podendo passar mais valores, como:

```css
p {
  font: italic small-caps bold 24px/2 Georgia, serif;
}
```

Ou seja, foi passado em ordem a font-style font-variant font-weight font-size/font-height font-family

## Textos

Existem diversas formatações de estilo de texto, a seguir algumas delas.

### Propriedade text-transform

Faz algumas conversoes de texto, por exemplo:

text-transform: capitalize

text-transform: uppercase

text-transform: lowercase

text-transform: none ou initial

text-transform: inherit (herdar do elemento pai)

### Alinhando o texto text-align

text-align: center

text-align: left

text-align: right

text-align: justify

### Colocando sublinhado com text-decoration

É possível adicionar um sublinhado no texto ou retirar o sublinhado de links com text-decoration

text-decoration-line ou text-decoration

text-decoration: none

text-decoration: underline

text-decoration: line-trought (traço no meio)

text-decoration: overline (linha em cima do texto)



text-decoration-style ou text-decoration:

text-decoration-style: solid

text-decoration-style: double

text-decoration-style: dotted

text-decoration-style: dashed

text-decoration-style: wavy



text-decoration-style-color:

Por padrão a linha segue a cor do texto, mas é possível estilizar com essa tag.

text-decoration-color: red



text-decoration-thickness: 5 px (a espessura do sublinhado)

### Identação de parágrafo com text-ident

Para definir o tamanho da identação de um parágrafo se utiliza text-ident:
​text-ident: 20px ou -20px

obs: essa propriedade aceita vários tipos de unidades de medida



### Propriedades letter-spacing e word-spacing

É possível separar cada caractere de um elemento utilizando letter-spacing.

letter-spacing: 2px ou -2px (definindo o espaçamento entre as letras)

word-spacing: normal ou 12px ou -12px (espaçamento por palavra do texto)



### Propriedade white-space

Essa propriedade define como funcionará o espaçamento de um texto de um <p> paragrafo por exemplo. Ele define algumas circuntancias como se o texto da tag terá exatamento o espaçamento definido, se o espaçamento fará encaixar no container que ele está dentro, etc.



### Propriedade word-wrap

Determina a quebra de linha, se ela será aplicada de forma que o texto não ultrapasse o width definido para o container ou se apenas será o texto passado sem respeitar o width.



### Propriedade word-break

Funciona de forma semelhante ao word-wrap, porém ele possui word-break: keep-all que se a palavra do texto for em chines, japones, coreano, etc, o texto é mantido sem quebra, pois nesses idiomas não se quebra linha na palavra.



## Sombras

### Sombra nos elementos

É possível colocar sombra interna e externa nos elementos. Isso com a propriedade box-shadow:
​

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trilha de CSS</title>
    <style>
        div {
            width: 200px;
            height: 200px;
            border: 10px solid #8f382e;
            margin: 20px auto;
            background: #fa8072;
            box-shadow: 10px 10px 10px red;
        }
    </style>
</head>
<body>
    <h1>Propriedade <code>shadow-box</code></h1>
    <div></div>
</body>
</html>
```

### 

passado o tamanho de cada lado da borda, a cor e um desfoque para a borda.



É possível também utilizar filter: drop-shadow(10px 10 px 5px gray) para aplicar um filtro nos elementos da imagem.

### Propriedade text-shadow

Também se pode colocar sombra nos textos. Em um h2 por exemplo e ele funcionará de forma semelhante ao box-shadow



