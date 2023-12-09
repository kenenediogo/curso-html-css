# Curso de Criação de Sites com HTML, CSS e JavaScript

# AULA 003: IMAGENS
EX 003: inserir imagens no site a partir de 3 fontes. A partir da mesma pasta, a partir de outra pasta, e a partir de uma fonte externa (Neste caso foi a partir de um site - URL)

<!-- Inserir imagens a partir da mesma pasta -->
< img src="logo-html.png" alt="Logo HTML" >

<!-- Inserir imagens a partir de uma pasta dentro da pasta -->    
< img src="imagens/logo-css.png" alt="Logo CSS" >

<!-- Inserir uma pasta a partir de um site com um URL -->
< img src="https://tkssharma.com/static/1bbde74a918ac99b9e7319e041cb62b5/714e6/js.png" alt="Logo JavaScript">

# AULA 004: Ícones
EX 004: Existem várias formas para criar FAVICON de um site. A que eu mais gostei foi usando o site favicon.ico, onde podemos criar icones de três formas: A partir de um texto, a partir de uma imagem e a partir de emojis.

Para inserir o mesmo, basta inserir um link:favicon na tag <head> por cima do <title> a tag <link rel="shortcut icon" href="html.ico" type = "image/x-icon">

# AULA 006: Hierarquia de Títulos
EX 006: Para criar a hierarquia dos títulos é necessário inserir as tags <h1> até a <h6>

# AULA 008: Formatação - Negrito e Itálico

Quando quisermos negritar, não usamos <b>xxx</b> passamos a usar os <Strong>xxx</strong> e no itálico, já não usamos <i>xxx</i>, mas sim <em>xxx</em>. 

Usamos a tecla de Atalho Ctrl + Shift + P, para abrir o Wrap with abbreviation, para podermos colocar as tags de forma mais rápida, sem ter que estar constantemente abrir e fechar.

Outras Formatações:

EX 008 - CÓDIGO FONTE: São partes de um código.

O código fonte de um site é o conjunto de instruções em linguagem HTML (Hypertext Markup Language) que define a estrutura e o conteúdo de uma página da web. Basicamente, é o “esqueleto” de um site, contendo todas as marcações e comandos que ditam como a página deve ser exibida no navegador.

<code> <!-- Ao fazer simplesmente o code ele perde a indentação -->
    num = int(input('Digite um número'))
    if num % 2 == 0:
        print(f'O número {num} é PAR)
    else
        print(f'O número {num} é ÍMPAR)
    print('Fim do programa')
</code>

<pre>
    <code> <!-- usando assim, ele vai indentar, mas vai colocar o texto com as tabulações e na pagina vai aparecer mais a esquerda -->
        num = int(input('Digite um número'))
        if num % 2 == 0:
            print(f'O número {num} é PAR)
        else
            print(f'O número {num} é ÍMPAR)
        print('Fim do programa')
    </code>
</pre>

BLOCKQUOTE: é para criar sitações extraidas de um livro, por exemplo algo que alguém escreveu e nós queremos fazer referência desta frase. Então usamos a blockquote, escrevemos a passagem dentro do < blockquote > e usamos um parâmetro dentro dela cite="": < blockquote cite="" > e dentro deste colamos o link do site.

# AULA 009: LISTAS ORDENADAS E LISTAS NÃO ORDENADAS

LISTAS ORDENADAS: Para usar as Ordered List, usa-se a tag < ol > para delimitar a lista e < li > (list item) para identificar cada item da lista. A tag < ol > possui um parâmetro type, onde configuramos o tipo de marcador da lista atual. As opções de valores para esse parâmetro são:

‣ 1 - Valor padrão. Cria listas numeradas. Ex: 1, 2, 3, 4, …
‣ A - Cria listas alfabéticas em maiúsculas. Ex: A, B, C, D, …
‣ a - Cria listas alfabéticas em minúsculas. Ex: a, b, c, d, …
‣ I - Cria listas com algarismos romanos em maiúsculas. Ex: I, II, III, IV, …
‣ i - Cria listas com algarismos romanos em minúsculas. Ex: i, ii, iii, iv, …

Também podemos indicar o início da contagem usando o parâmetro start. Por exemplo, a tag < ol type=“I” start = “5” > vai gerar itens numerados como V, VI, VII, VIII, IX, … 

LISTAS NÃO ORDENADAS: Para criar uma unordered list, vamos usar a tag <ul> para delimitar a lista e a tag <li> para criar cada um dos seus itens internos. O marcador padrão é a bolinha preta totalmente preenchida (circle), mas existe a opção de configurar a propriedade type da tag <ul> com os seguintes valores:

‣ disc - padrão. Uma bola preta totalmente pintada
‣ circle - Uma bola com uma borda preta e sem preenchimento
‣ square - Um pequeno quadrado preto totalmente pintado

LISTAS DE DEFINIÇÃO

dl - Definiction List (Lista de Definição):
dt - Definiction Term (Termo de Definição):
dd - Definiction Description (Descrição da Definição):

<dl>
    <dt >HTML</dt>
    <dd>Linguagem de marcação utilizada para criar o conteúdo do site.</dd>
</dl>

# AULA 010: LIGAÇÕES EM TODA PARTE

Para criar um hyperlink, devemos criar âncoras através da tag <a>. O principal atributo dessa tag é o href, que cria uma referência hipertexto,  dentro do atributo href, o que colocamos foi uma URL completa para outro site.

Para poder controlar onde o site de destino vai abrir, podemos usar o atributo target, que suporta os seguintes valores:
‣ _blank: vai abrir o link em uma nova janela em branco
‣ _self: vai abrir o link na janela ou frame atual (padrão) 

* Ligações Externas: <a href="https://www.facebook.com/kenenediogo98" target="_blank" rel="External" >minha conta do facebook</a>
* Ligações Internas: <a href="noticias/pag003.html" rel="next" target="_self">Terceira página (notícias)</a>

para efetuar download de algum material em PDF, ou de um arquivo ZIP qualquer. Aqui vão alguns media types bem usados no nosso dia-a-dia:
‣ application/zip       ‣ text/html     ‣ text/css      ‣ text/javascript       ‣ video/mp4         ‣ video/H264            ‣ video/JPEG
‣ audio/aac             ‣ audio/mpeg    ‣ font/ttf      ‣ image/jpeg            ‣ image/png

* Links para Download: <a href="livro/10 - Ligações em toda parte.pdf" download="10 - Ligações em toda parte.pdf" target="_blank" type="application/pdf">Baixar o livro em PDF</a>

Existe um recurso bem interessante para links que é indicar qual é a natureza do destino usando o atributo rel. Esse atributo aceita vários valores, entre eles vou citar:

‣ next indica que o link é para a próxima parte do documento atual
‣ prev indica que o link é para a parte anterior do documento atual
‣ author indica que é um link para o site do autor do artigo atual
‣ external indica que é um link para outro site que não faz parte do site

# AULA 011: MÍDIAS (FOTOS E AUDIOS)

Aula 011: FOTOS

<picture>
   <source media="(max-width: 750px)" srcset="imagens/foto-p.png" type="image/png">
   <source media="(max-width: 1050px)" srcset="imagens/foto-m.png" type="image/png">
   <img src="imagens/foto-g.png" alt="Imagem flexivel">
</picture>

É importante que existe uma ordem entre os <source>, e nessa nossa configuração, os itens mais acima sejam os menores tamanhos para max-width e que os seguintes sejam maiores, de forma crescente. O último item dentro de <picture> deve ser a imagem padrão.

Note que a tag <source> possui três atributos:

‣ type: vai indicar o media type da imagem que usamos (veja mais informações sobre media types no capítulo 10).
‣ srcset: vai configurar o nome da imagem que será carregada quando o tamanho indicado for atingido.
‣ media: indica o tamanho máximo a ser considerado para carregar a imagem indicada no atributo srcset.

Aula 011: AUDIOS

<audio preload="metadata" autoplay controls>
   <source src="midia/guanacast-33.mp3" type="audio/mpeg">
   <source src="midia/guanacast-33.ogg" type="audio/ogg">
   <source src="midia/guanacast-33.wav" type="audio/wav">
   <p>Infelizmente seu navegador não consegue reproduzir áudio. </p a href="midia/guanacast-33.mp3" >baixar o arquivo MP3</a></p>
</audio>

Vamos analisar os principais atributos da tag <audio> antes de mais nada:

‣ O atributo preload: indica se o áudio será pré-carregado ou não e aceita três valores:
๏ metadata: vai carregar apenas as informações sobre o arquivo (tamanho, tempo, informações de direitos, etc)
๏ none: não vai carregar absolutamente nada até que o usuário clique no botão play ou um script inicie a reprodução
๏ auto: (padrão) vai carregar o arquivo de áudio inteiro assim que a página for carregada, mesmo que o usuário nunca aperte o play

‣ O atributo controls: vai apresentar o player na tela. Caso não seja colocado na tag < audio >, o controle será transparente e o usuário não poderá interagir com ele.
‣ O atributo autoplay: quando inserido, vai iniciar a reprodução do áudio assim que a página for carregada.
‣ O atributo loop: vai fazer com que o áudio seja repetido eternamente assim que terminar a sua reprodução.

Dentro da tag < audio >, adicionamos vários < source > com formatos diferentes do mesmo áudio. Coloque na parte de cima o seu formato favorito. Os demais só serão carregados caso o de cima falhe. Caso todos falhem, criamos um parágrafo que permite o download do arquivo MP3 para ouvir no player padrão do dispositivo.

# AULA 012: VÍDEOS

VÍDEOS

<video width="500" poster="imagens/limoes-capa.png" controls>
    <source src="midia/meu-video.mp4" type="video/mp4">
    <source src="midia/meu-video.m4v" type="video/mp4">
    <source src="midia/meu-video.webm" type="video/ogg">
    <p>Seu navegador não tem compatibilidade com a reprodução de vídeos</p>
</video>

Atributos importantes ta tag video:

‣ width: vai indicar a largura que o vídeo vai ter na tela. Nesse exemplo, 600px.
‣ poster: configura uma imagem que vai aparecer como uma capa, enquanto o visitante não aperta o play para reproduzir o vídeo
‣ controls: vai configurar se os controles do vídeo vão aparecer na parte inferior da mídia. Por padrão, os controles não aparecerão, mas basta colocar a palavra controls na tag < video >.
‣ autoplay: diz para o navegador se o vídeo vai começar a tocar automaticamente, assim que a página for carregada.
‣ loop: vai reproduzir novamente o vídeo assim que ele terminar

# AULA 013: ESTILO INLINE

O Estilo inline, significa fazer a estilização nas tags HTML com CSS na própria linha.

<body style="background-color: lightskyblue; font-family: Arial, Helvetica, sans-serif; font-size: 20px;">

    <h1 style="color:mediumblue; background-color: dodgerblue; font-size: 1.5em;">Capítulo 1</h1>
    <h2 style="color: darkred; font-size: 1.2em;">Capítulo 1.1</h2>
    
    <h1 style="color:mediumblue; background-color: dodgerblue; font-size: 1.5em;">Ca
    <h2 style="color: darkred; font-size: 1.2em;">Capítulo 2.1</h2>
    
    <p style="text-align: justify;">Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci delectus debitis eligendi cumque quis consequuntur! Quas, velit dignissimos provident minima cumque, sed cum ab inventore ipsum natus ipsa error reiciendis.</p>

# AULA 014: ESTILOS LOCAIS / INTERNOS

A esitização do texto é feita dentro da Tag <Head>, com a tag:

 <Style>
    body{
       background-color: blue;
      }
</style>

# AULA 015: Estilos Externos ESTILOS EXTERNOS

@charset "UTF-8";

body{
    background-color: lightsteelblue;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 20px; }

h1{
    color: darkblue;
    background-color: lightblue; }

h2{
    color:darkred }

p{
    text-align: justify; }

a{
    text-decoration: none; }

# AULA 016

REPRESENTAÇÃO DE CORES:

Podemos fazer a representação de cores de tres maneiras:

<!-- Representação por códigos Hexadecimais; Decimal: 0 1 2 3 4 5 6 7 8 9; Hexadecimal: 0 1 2 3 4 5 6 7 8 9 A B C SD E F -->
<h2 style="background-color: #0000ff; color: #ffffff";">Exemplo de Cores 2</h2>

<!-- Representação por Código RGB (Red,Green, Blue) -->
<h2 style="background-color: rgb(0, 0, 255); color: rgb(255, 255, 255);">Exemplo de Cores 3</h2>

<!-- Representação por Características de Cores: (Hue(matis), Saturation(saturação), Luminosity(luminosidade)) -->
<h2 style="background-color: hsl(240, 100%, 50%); color: hsl(0, 0%, 100%);">Exemplo de Cores 4</h2>

GRADIENTES (DEGRADE):

Para usar um gradiente, temos que usar a propriedade: "background-image", com a propriedade: "liner-gradient", e os seus atributos: "to right, white, blue", podemos usar também "to left", "to right", "to top", "to bottom", ou ainda usar em graus: 90deg, 45deg, -45deg, -90deg etc. Podemos ainda adicionar a percentagem de ocupação da cor a frente do código da cor.

<style>
        
	* { /* Configurações globais em CSS */
        	height: 100%;
       	}

        body{ /* para inserir gradiente, tem que usar essa propriedade: Background-image, com a propriedade: linear-gradient
            		
		background-image: linear-gradient(to right, #7A0FFF 1%, #C500FA, #FF00C3, #FF6500, #FFC300);
            	background-image: radial-gradient(circle, #7A0FFF, #C500FA, #FF00C3, #FF6500, #FFC300);
            	background-attachment: fixed; /* fundo fixo */
        }

</style>



