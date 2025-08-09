# HTML

HTML é um arquivo de texto de marcação, ele possui tags que são interpretadas pelo navegador para fazer delimitações e funções específicas.

## Inspetor de elementos

O inspetor de elemento é uma ferramenta de desenvolvedor presente nos navegadores, com ele você tem diversas funcionalidades como visualizar o html da página que está sendo acessada.

Para acessa-lo basta apertar f12 ou nas opções do navegador.



## Como consiste um arquivo html

### Tags

O HTML consiste em 3 partes:

**Tag <html>**: Toda tag possui o sinal de menor <, sinal de maior >  e a tag dentro desses sinais.

Toda tag também possui o seu fechamento:

</html>: Isso é justamente a marcação da linguagem, o **<html>** delimita o início do bloco e o </html> delimita o fim.

<head> e <body>: O body é aquilo que será exibido para o usuário na página, já o head são coisas que não serão exibidas ao usuário na página.

Um exemplo de head seria a tag <title> que é o titulo da página.

ex:


[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/d215a9a5-d03b-4a16-bae7-34f712ece97f)

É possível observar que o title que fica dentro do head é o titulo da página na aba, já o body se tornou o texto na página

tag <i>: Essa tag deixa o texto em itálico <i>Meu primeiro html</i>

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/45e0a635-6945-4bca-a931-2d916cbefd7a)

tag <strong>: Essa tag deixa o texto em negrito:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/1541bdd3-3c96-4575-a02c-94a28ac213ea)


É possível utilizar duas tags ao mesmo tempo, como colocar em negrito e itálico ao mesmo tempo

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/612c5a3c-8251-444a-b0e4-d3e3c240f274)

É possível deixar um texto em strong e apenas uma parte dele em itálico:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/ed60bb5c-c751-4b79-9e80-bbb8d3b30485)

### Tags sem fechamento

É possível ter tags sem fechamento.

Já foi visto que as tags geralmente possuem <tag> de abertura e </tag> de fechamento porém algumas tags podem não ter fechamento.

Um exemplo disso é a tag <input>

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/856b202d-6fc3-4ca4-8ede-3af70fd455a5)

Outra tag pode ser a <img> para inserir imagem.

## Atributos das tags

Como foi visto no caso de <input> existe o "type="text"", esse type é um atributo da tag

Atributos são propriedades que uma tag pode ter, podendo ter atributos mais genéricos (que várias tags podem ter) e atributos mais específicos de cada tag.

#### Atributos gerais

Na tag <strong> por exemplo é possível ter o atributo "id", o id é utilizado para quando for utilizado o JavaScript, a linguagem de programação alterar o conteúdo dele:

<body>

        <strong id="titulo">Meu primeiro <i>html</i></strong>

        <input type="text">

    </body>

Outro exemplo é o atributo style, o style pode ser usado tanto em css quanto JS, mas geralmente em CSS. O CSS é uma forma de formatar o html, mudando seu estilo e aparência:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/250b4a86-5396-40f8-a47a-c025471d896e)

No exemplo <strong style="color: blue">Meu primeiro <i>html</i></strong> é utilizado o style para o css alterar a cor da tag para azul.

Outro atributo gerais das tags é class, ela serve para ser aplicado um determinado estilo css em uma série de tags com essa classe, por exemplo:

<strong class="titulo-principal">Meu primeiro <i>html</i></strong>

Desta forma, toda tag da classe "titulo-principal" terá um determinado comportamento, como uma cor específica, sem precisar colocar um identificador id em todas as tags.



#### Atributos específicos da tag

Como foi citado, alguns atributos são específicos da tag, no caso do <input> por exemplo, essa tag pode receber inputs de vários tipos, cada um com um formato diferente.

Já foi visto com type-"text", mas também é possível utilizar "number" para o input receber somente numeros, ou "color" para inserir uma cor:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/b65ca268-592d-45fe-a5f5-0fb47b0eac2d)

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/8232f4ab-f55f-4524-ba09-7fdb2721a961)

Outra tag com atributos específicos é a <img>, ela precisa de um atributo chamado "src" que é o caminho da imagem, pode ser um caminho da web ou um caminho da máquina sendo utilizada. 

Exemplo:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/6fba1117-01ca-49bb-aec8-e1d57459b7ce)

Nesse exemplo foi pega uma imagem do google passando o endereço da imagem no atributo "src"

Como foi visto, a imagem ficou muito grande na página, então pode-se usar o atributo "width" para selecionar o tamanho da imagem:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/7c691954-0087-4941-8820-1a56a3f8fc1a)

## Tags de texto

No HTML existe uma variedade imensa de tags de texto, algumas delas são:

tags h(h1,h2,h3,...):

Essa série de tags indicam títulos, no caso H1 seria o titulo, h2 um subtitulo, h3 um titulo dentro do título e assim por diante.

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/7ede2ed5-295c-49a6-8527-05bdcbc349ad)

Já para parágrafos é utilizada a tag<p>:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/64bc8caa-c714-41e5-9c3d-982416c7be32)

OBS: O próprio navegador reconhece as tags e adiciona um determinado espaçamento entre linhas para cada tag e isso pode ser determinado também pelo css.


​Para citação é utilizada a tag <blockquote>

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/0286df91-ab13-45e8-a73e-29636e5fa286)

Isso pode ser tanto uma observação quanto uma citação, o navegador ainda adiciona uma margem para essas tasgs.

É possível utilizar <u> para adicionar um underline no texto:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/74e136f1-057e-41a0-8164-80500eed54c7)

Ou mark para deixar com um marca texto:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/b4ae412a-1f4c-46be-8433-68c6c5c91df6)

Ou colocar uma notação no texto com <sup>:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/27f6be47-a606-47d6-8e06-afe0869b5608)

## Listas

Listas é uma forma que o navegador interpreta para separar tópicos, sequencias, entre outros.

O HTML possui duas principais listas, as ordenadas e as não ordenadas.

listas ordenadas são feitas com a tag <ol> </ol>, essa tag em específica não funciona colocando seu conteúdo simplesmente dentro dela, como <ol>Uma lista</ol>.

As listas precisam de uma tag filha, que pode ser <li></li>

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/feee82e4-672b-43b5-9ed7-612875e4c610)

Também sendo possível colocar uma lista dentro de outra lista:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/adbc1bc6-e62b-42f8-9f0b-528d3ceb76da)

Já a lista não ordenada ela tem itens apenas com marcadores, sem numera-los ou ordena-los utilizando a tag <ul> invés de <ol>:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/82482978-8383-427d-afcd-b6c7afae4b79)

A lista não ordenada geralmente é utilizada junto ao css para fazer menus.

## Links

Geralmente em sites existem links para se redirecionar a outra página web, issoo pode ser feito utilizando a tag <a>, nela você adiciona o atributo "href" que recebe o link da outra página, já o conteúdo dentro da tag é um texto que vai ser clicado:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/ce58d32f-622d-4c27-ae5c-3848c21ac751)

Assim, na mesma aba você é redirecionado a outra página web, um atributo que pode ser utlizado para definir o comportamento de onde será aberta a página quando clicar no link, se na mesma aba ou numa nova é o target=

Por padrão, o target é "self", e pode ser explicitado isso, mas pode também ser como "_blank" o link é aberto numa nova aba

<a href="[http://dio.me](http://dio.me)" target="_blank">Dio</a>

Outro atributo da tag <a> é o title=, ele serve para adicionar um tooltip no link, que é ao passar o cursor do mouse em cima do link aparece uma mensagem por exemplo.

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/9123b4d8-7901-4328-8ef6-6af1d078e47e)

É possível transitar entre duas páginas html

Em index:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/b7179f4a-6218-4453-bace-09cdb37fd324)

Em about:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/ac623572-3ea3-4e11-8e7c-3ddf949d4367)

# Formulários html

Formulários é a base para preencher campos e trabalhar com dados em html

para criar formulários, primeiramente é utilizada a tag <form>, porém

O código puramente assim

</head>

<body>

    <form>

        Este é o formulário

    </form>

</body>

</html>

não gerará um formulário, pois a tag form no html precisa da tag de input

Agora com a tag input:

<body>

    <form>

        Nome: <input type="text" name=""><br>

        Idade: <input type="number" name=""><br>

        Senha: <input type="password    " name=""><br>

    </form>

</body>

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/68a4ca60-daa5-44f8-8150-7b7ce1ad8071)

Também é possível usar a tag <button> com o atributo "type" como submit

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/c6a61ffc-60f1-4712-a6d8-46607a8b245a)

    <form>

        Nome: <input type="text" name=""><br>

        Idade: <input type="number" name=""><br>

        Senha: <input type="password    " name=""><br>

        <button type="submit">Enviar</button>

    </form>

Assim já se obtem um formulário, conseguindo inserir texto no Nome, números no campo idade e senha com **** no campo Senha. Além de ter um botão de enviar.

Também pode se colocar nome no formulário, com <form name\="signup"\>, essa nomeação servirá para identificar os elementos com o JavaScript também para fazer validações.

Também é possível adicionar o atributo action= que recebe o endereço onde será enviado o formulário.

Outro método para o form é o method=, que recebe os métodos de api do protocolo http (get,post,put,delete), ex:

<form name\="signup" method\="GET" action\="#"\>

Quando o formulário for preenchido, a url mudará para:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/27be0df4-7861-45d2-be68-2e51492c605f)

Ou seja, ele já deixará um query/json pronta para consultar na api/banco de dados. Um detalhe é que a senha apareceu na url, o que é inseguro, pois o certo é colocar a senha em um método post.

O método post manda a requisição por um body que não utiliza a url.

Outro atributo é o target, que funciona igual ao target de abrir um link, quando clicar no button a consulta será feita em uma nova aba.

Outro atributo é o autocomplete, ele recebe "on" ou "off", basicamente ele onn faz com que quando o usuário volte a página do formulário ele não precise colocar as credenciais todas novamente, só a senha.

É possível adicionar um evento, para isso existem os atribuitos on..., que fala como a tag vai se comportar ao fazer alguma ação, por exemplo:

onsubmit="alert('Enviei o form')"

Ao clicar em submit ele exibe um alerta dizendo que enviou o formulário:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/a44b1254-8d06-4500-873f-6af19842d121)

Isso pode ser utilizado por exemplo para "formulário".

# Tag input

A tag input possui o atributo type, que são os tipos de input para essa tag, alguns são:

text = campo de texto comum

number = O tipo numero, o navegador já cria uma setinha para adicionar ou subtrair números, que pode ser controlada, ex

<label>Number:</label><input type="number" min="0" max="99" step="5">

Aqui o min determina que o minimo que a seta chega é zero, sem números negativos

max determina que o máximo do campo é 99

step determina que a seta vai aumentar de 5 em 5 numeros.

Button = Um botão para fazer alguma ação, geralmente enviar o formulário

O tipo button cria um botão, mas da mesma forma é possível utilizar a tag <button>

 <label>Button:</label><input type="button" value="ENviar">

<button type="button">Enviar</button>

Ambos são iguais.

range = Um controlador para definir algum range numérico:

<label>Range:</label><input type="range" min="0" max="100" value="10">

min diz que o minimo dele é 0 e max que o máximo é 100

value determina que ele comece em 10 por padrão, na página:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/2eb2b3d6-d905-4d67-92c6-f8760f39278d)

color = Abre um editor de cor

<label>Color:</label><input type="color">

email = Ao enviar o formulário esse campo adiciona um popup caso não haja @:

 <label>Button:</label><input type="submit" value="ENviar"><br>

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/8e0701b0-bdaa-4ce0-9f5e-da1ef3232d61)

url = Faz a mesma coisa que o atributo email só que para formatar url colocando também o http:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/518ecee0-9bc5-4914-924b-c2f401c656f9)

date = Possíbilita um calendário para selecionar a data:

 <label>Date:</label><input type="date"><br>

week = Permite selecionar o número da semana, com um calendário do lado (apenas no chrome e edge)

        <label>week:</label><input type="week"><br>

month = Permite selecionar o mês e o ano, ex: outubro de 2019, com um calendário:

        <label>month:</label><input type="month"><br>

checkbox = Uma caixinha para seleção (true e false):

        <label>Checkbox:</label><input type="checkbox"><br>

radio = Quando colocado duas tags radio você seleciona ou um ou outro, semelhante ao checkbox mas aqui a escolha é única:

        <label>radio:</label><input type="radio" name="aceita"><input type="radio" name="aceita"><br>

lembrando que para isso precisa estar um do lado do outro e com a tag "name"

<body>

    <form>

        <label>Text:</label><input type="text"><br>

        <label>Number:</label><input type="number" min="0" max="99" step="5"><br>

        <label>Button:</label><input type="button" value="ENviar"><br>

        <label>Range:</label><input type="range" min="0" max="100" value="10"><br>

        <label>Color:</label><input type="color"><br>

        <label>E-mail:</label><input type="email"><br>

        <label>URL:</label><input type="url"><br>

        <label>Date:</label><input type="date"><br>

        <label>week:</label><input type="week"><br>

        <label>month:</label><input type="month"><br>

        <label>radio:</label><input type="radio" name="aceita"><input type="radio" name="aceita"><br>

        <label>Button:</label><input type="submit" value="ENviar"><br>

    </form>

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/124a488b-1565-41c6-a1f1-5af07c084fe1)


## Checkbox e radio

Dois tipos de inputs muito importantes são de checkbox e radio, pois eles precisam de algumas lógicas e formatações específicas a serem seguidas.



### Campo name em checkbox

No seguinte formato, em todos os checkbox o campo name possui o mesmo valor e o campo value possui os seus valores respectivos de texto:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/fa9fbdb9-1a4d-4a56-a8f4-84a9902528b3)

Porém, ao selecionar esses campos no checkbox e enviar o formulário, o modelo gerado é o seguinte:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/0db47916-2431-4a81-b07b-f4db61969f1c)

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/81931aa2-f252-4fef-8b2d-27e8cb4452cc)

Todos os atributos/chaves estão como opcional, isso significa que no momento que isso for mandado a api do backend, ele pegará apenas o último valor "azeitona", pois todos são iguais.

A forma de corrigir isso, seria da seguinte forma:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/d319aa3b-f6bd-4a6c-b1ff-73e52edd744f)

Utilizando o método post invés de get e ao lado de opcional colocar colchetes [], assim o backend entende que será passado uma lista de $opcional['queijo','cebola','azeitona'']



Um outro problema pode ser no radio, se o atributo name for igual, ele permitira selecionar as duas opções

Ou seja, é imprescindível que seja adicionado name= e value= para os campos de input.



## Button

A tag button pode ter diversos comportamentos utilizando o atributo type como button e os atributos on..., por exemplo onmouseover= acontecerá algo ao passar o mouse em cima do botão (essas coisas podem ser feitas com qualquer elemento usando html)

Se o type do button for "reset" ele limpa os campos do formulário

Já o type submit ele envia o formulário para algum lugar. Ele também gera na url dados de atributos "index.html?name=dfds&age=-9&password=fdsf". O formulário trabalha junto com o button com tipo submit, pois é possível utilizar um atributo no FORMULÁRIO (tag form) chamada onsubmit, para validar  os campos por exemplo.

No formulário <form> é possível usar o atributo onsubmit ou outra orientação a enventos, que pode ser feita alguma ação a partir do formulário antes de enviar de fato (isso quando clicar no botão de submit



### Select

Select box é um campo que tem uma lista pré definidas com opções para input.

Um exemplo de caso é um campo "cargo", geralmente em cargo você já tem opções pré definidas como desenvolvedor frontend, desenvolvedor fullstack, etc.



```html
<body>
    <form onsubmit="" method="get">
        <label>Cargo:</label>
        <select name="role">
            <option value="">Selecione o cargo</option>
            <option value="administrativo">Administrativo</option>
            <option value="gerente">Gerente</option>
            <option value="diretor">Diretor</option>
        </select>

    </form>
</body>
```

O select geralmente possui um nome, no caso role e a tag <option> para auxiliar, as opções tem as opções a serem escolhidas, essa tag ainda precisa do atributo value= para saber o valor que será mandado ao backend. Ficando assim:

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/406f35b4-d39b-43a7-b818-95ca51a7031f)

Essa tag é muito importante para o javascript, principalmente em relação ao campo "onsubmit" do form.

### textarea

Essa tag serve como uma caixa de texto para textos mais longos. O tamanho dessa caixa pode ser editado pelo usuário ou determinado pelo html.



## Estruturando e formatando o HTML

Uma das coisas mais importantes quando se fala de HTML é estruturar de uma forma que fique fácil de fazer alterações e compreender o que está sendo feito.

Quando for ser aplicado o CSS por exemplo o html já deve estar estruturado corretamente.

### Formatação

Além disso o HTML deve ser semântico, que é basicamente o HTML ter a interpretação da mensagem que deve ser passada. Por exemplo usar a tag <strong> ou invés de <b> para deixar em negrito, isso devido a em alguns casos o texto em negrito carregar uma outra entonação além de apenas deixar o texto escuro e destacado.

É possível também formatar o html utilizando a tag <font>

a tag font tem alguns atributos:

color= definir a cor, ex color="red"

face= seria a fonte do caractere, ex face="arial"

o atributo face também pode receber mais de uma fonte, para caso o usuário não tenha aquela primeira fonte em seu navegador, ex: face= "arial, Trebuchet"

### Estrutura

A principal forma de estruturar a página html é com a tag div e a tag span

<div> - A tag div serve para separar a página em blocos, dividindo a tela em partes de conteúdo.

Geralmente ela não possui atributos, apenas o id para ser identificada pelo Java Script, uma forma de iniciar a desenvolver uma página é pela estrutura das divs (onde ficará o menu, tamanho do cabeçalho, conteúdo, etc)

A div é considerada uma tag do tipo display-block, o que significa que ela ocupa a tela inteira horizontalmente

<span> - A tag span é semelhante a div, mas ela separa apenas o elemento que está dentro dessa tag. Por exemplo: É possível colocar na tag span apenas um caractere para fazer uma ação específica "frase para <span>colocar</span> o span".



<fieldset> - Essa tag serve para fazer uma separação visível do bloco e possibilitando colocar uma legenda colocando uma tag <legend>

[image](https://app.capacities.io/78c08dc6-c06f-4366-8edd-ba7149376027/1928c85f-644e-4875-a69f-492eafcecdfa)


<video> - Uma tag para colocar videos (ex: mp4)

<iframe> - Utilizada para colocar uma outra página/site dentro da sua página, possíbilitando a navegação em duas páginas, uma dentro da outra.



## Html Semântico

Semântica quando relacionada ao HTML é devenvolver uma página com tags que façam sentido. Por exemplo, anteriormente em páginas era muito comum encontrar muitas divs para estruturar o código.

Porém, com o html semântico, a melhor prática é estruturar a página com as suas respectivas tags (header, main, footer).

Isso pode contribuir de diversas formas para a página web, com acessibilidade e Web Scraping.

Web Scraping - É coletar dados da página web com algum robô (selenium por exemplo).



### Header, main e footer

Header é o cabeçalho

Main é a tag onde ficará o foco principal da página. Não pode ser usado duas vezes na mesma página. Ela deve ser filha apenas de uma div ou de uma body

footer o rodapé



#### Nav, Aside e section

section - Semelhante a div, separa sessões da página

aside - é um conteúdo separado do conteúdo principal da página. Nunca deve ser usado para texto entre parêntese. Pode ser usado em uma barra lateral ou um box com biografia dou autor.

nav - é uma sessão de navegação, onde devem ficar os links como por exemplo links para outras páginas, "sobre nós", etc. geralmente é usado lista não ordenada como tag filha.



#### Article, blockquote e q

article - É uma tag para colocar o artigo da página. Ele pode possuir aninhamento com vários articles. Pode ser utilizado junto com a tag  <time> com o atributo "datetime" ou "pubdate" para definir a data de publicação do artigo.

blockquote - É uma tag utilizada para citação, por exemplo: Possui um parágrafo (tag "p") falando sobre um tema, logo em seguida a citação desse parágrafo. Podendo colocar fonte atravéz do atributo  "cite="

q - Uma citação apenas para um trecho específico, podendo também utilizar "cite="



#### Figure, Figcaption e Picture

figure - A tag figure serve como uma div container. Dentro dela é usada a tag <figcaption> que serve como legenda para uma imagem colocada anteriormente com a tag <img>

picture - A tag picture é parecida com a figure, mas com essa é possível utilizar uma tag <source> e passar alguns atributos para ela, que são "srcset=" e "media=". Isso serve para definir uma outra imagem em "srcset" que será renderizada quando o tamanho minimo de "media" por exemplo "media="(min-width: 600 px)"" então quando a tela do dispositivo no navegador estiver menor que 600 pixels, o navegador trocará a imagem definida na tag <img> para a tag definida no atributo "srcset=" da tag source.

#### SEO

SEO (Search Engine Optimization / Otimização para mecanismos de busca)

O SEO engloba um conjunto de técnicas para otimizar o posicionamento do site em mecanismos de buscas.

Uma boa forma de avaliar como está o SEO do seu site é o Google Search Console. Nele possui métricas para avaliar as buscas e os acessos do seu site.

dicas para SEO:

Utilizar de 50 a 60 caracteres na tag title da página.

Usar a tag meta na headers da página com o atributo "name=" como "description" e a tag "content=" com alguma descrição.

usar o site Schema.org


# CSS

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
