# HTML: O que é?

#### HTML é uma estrura de marcação, utilizado para estruturar páginas web, quando falamos de HTML é como imaginar uma pessoa que para se manter em pé necessita de um "esqueleto", assim é uma página web.
#### A sigla HTML significa "HyperText Markup Language", ou seja, um hipertexto de marcação, isso quer dizer que usamos o HTML como base estrutural para marcar partes de uma página web.

## Como criar a primeira página Web?

É muito simples, o HTML pode ser escrito em uma IDE, como Visual Studio Code, ou então, em um bloco de notas.
Basta criar um arquivo e salvar com a extensão .html, exemplo:
 `meuSite.html` <br>
Agora é simples, basta ir na pasta que foi salva e abrir o arquivo, note que ao fazer isso, abre seu navegador com uma página em branco.
<br>"Será que deu errado? não apareceu nada."<br>
Na verdade, deu muito certo, sua página **HTML** ja está ativa "localmente", agora é mão na massa para escrever a estrutura básica.

# Estrutura Básica: 

Como dito acima, o HTML é um Hipertexto de marcação, então ele precisa de palavras-chave para fazer suas marcações na página.
Essas palavras-chaves chamamos de `TAG`. <br>
As TAG's serve para definir partes da estrura, voltando com exemplo de corpo humano
foi dito que o HTML é como um esqueleto, as TAG'S para nós, seria partes desse esqueleto como: costela, vertebra, crânio etc;
cada parte do nosso esqueleto tem uma função e um local especifico, e no HTML não é diferente.

 ### Como tag possuímos várias, mas vou listar as principais:
  - **\<title>**: É onde escrevemos o título da nossa página, ou seja, o nome que aparece na aba do navegador.
  - **\<html>** : Tudo que escrevemos no HTML precisa estar dentro dessa tag principal, que vai sustentar todo o esqueleto
  - **\<body>** : É a parte principal da página, onde tudo é escrito e exposto de forma principal.
  - **\<head>** : É o cabeçalho da nossa página, mas por padrão pe utilizado para adicionar plugins e outros mecanismo.
  - **\<p>** : Essa tag é responsável por definir um parágrafo (Bloco de palavras)
  - **\<h1>** : H1 é o tamanho da letra, quanto menor o número, maior a letra, pode ser usado para destacar títulos.
  - **\<a>** : Essa tag é super interessante, com ela podemos integrar links ao nosso site, tanto externos como internos.
  - **\<ul>** : Cria uma lista desordenada, ou seja, itens um embaixo do outro com marcação.
  - **\<li>** : Pode ser entendido como list-item, ou seja, o item que vai estar dentro da nossa lista.
  - **\<ol>** : Uma lista ordenada, como numeração em cada \<li>

Mas sei que ainda parece confuso, por isso o melhor jeito de aprender é colocando em prática, mas calma, teorias são importantes nesse processo<br>
A grande maioria das tags necessitam de fechamento, o que quer dizer que você precisa declara-las novamente ao final com uma "/" por exemplo:

```
<h1>Olá, mundo!</h1> // O HTML só vai entender que você declarou aquela tag, quando ela for fechada
```
<br>"Mas qual o intuito de abrir e fechar?"<br>
<br>
A abertura de uma TAG é como um espaço que você abre para declarar algo, usando ainda o exemplo de corpo humano:<br>
Quando uma tag abre, imagine que está declarando uma parte do corpo, como braço por exemplo, nesse braço teremos vários outros ossos (tags) que juntos constituem a estrutura que chamamos de braço
<br>No HMTL abrimos uma tag, e dentro dela podemos declarar textos, imagens, parágrafos, lista etc, e ao fecharmos essa tag, ela conclui o fim daquela seção na página.<br>
Exemplo:<br>

```
<body>
  <h1>Olá, Mundo!</h1>
</body>
```

Veja como definimos o texto "Olá, mundo!" dentro de uma outra tag, chamada "Body", ao fechar o Body, avisamos ao HTML que entre a abertura e o fechamento está o conteúdo da nossa página.

## FORM

Agora que ja abordamos como funciona o HTML e suas TAG's, podemos abordar a tag mais usada no universo web.<br>
Estou falando da tag\<form>, ela serve para avisar ao navegador que naquela parte do site teremos um formulário, como formulário me refiro a tudo aquilo que envia dados ao servidor, sendo dados cadastrais ou de contato por exemplo. Quando acessamos redes sociais, ou fomulários na internet, existem campos a serem preenchidos, esse campos do fomulário são os \<input>, input é uma tag que é inserida dentro do formulário que especifíca que naquele local do \<form> teremos um entrada de dados:<br>
```
<form>
  <input type="text" id="username" name="username"><br> // Note que temos o tipo "text" específicado no input
</form>
```

Note como o input vai dentro do forms, definindo assim que naquela parte está um campo para entrada de dados, podendo ser de várias formas: texto, número, senha, data, semana, mês etc.<br>
São inumeras as possibilidades quando falamos de inputs, por isso vou apenas destacar as principais e mais vistas:<br>

- \<input type="text"> = Esse input cria em nosso navegador uma barra para escrever textos alphanuméricos, ou seja, numeros, letras e caracteres especiais.
- \<input type="number"> = Esse input fica restrito apenas a números, podendo ser limitado entre minimo e máximo.
- \<input type="reset"> = Esse input cria um botão clicável que limpa os dados escritos no fomulário em que ele esta inserido.
- \<input type="password"> = Esse input cria uma barra de texto, que ao escrever no apresenta **** par anão revelar o texto, ja que se trata de uma senha.
- \<input type="date"> = Esse input cria uma caixa de texto com um ícone de agenda, para que seja escolhido uma data, ele não aceita outras datas
- \<input type="month"> = Como o input de data porém só aceita meses como resposta.
- \<input type="button"> = Cria um botão clicável, que pode ser atribuido a alguma função específica via código
- \<input type="submit"> = Cria um botão com a função de enviar, ele envia os dados escritos no formulário.

Agora que conehcemos os input do formulário, quero destacar um em especifico, do tipo "submit", esse botão mencionado envia os dados do nosso formulário para o servidor.<br>
#### "Como ele faz isso?"
O submit usa como base para envio as informações inseridas no fomulário, desde que bem específicadas, vou explicar, a tag \<forms> tem atributos igual aos inputs, porém são atributos relacionados ao funcionamento geral<br>
```
<form name= "formulario" method="POST" action = "#"> 
  <input type="text" id="username" name="username"><br> // Note que temos o tipo "text" específicado no input
</form>
```

Veja como o formulário tem 3 atributos, sendo eles o:<br>

- name = Esse atributo define o nome do nosso fomulário, isso transforma ele em uma tag única e exclusiva, que para referenciar utilizamos o seu nome, ou comumente dito ID
- action = Esse atributo define para onde nossos dados serão enviados, aceitando links ou caminhos de diretório, podendo ser o link do servidor.
- method = Define de que forma os dados serão enviados, para isso temos duas opções: POST e GET.

### Method:
- POST = Nesse método os dados serão encapsulados como em um pacote e enviados via protocolo HTTPS, o que significa que serão criptografados e só serão abertos novamente pelo servidor, isso evita que alguém intercepte esse pacote e tenha acesso a dados sensíveis como senhas.
- GET = Esse método envia os dados via URL da página, o problema desse método é que ele expõe os dados no URL, ele é mais usado para registro temporários e não-sensíveis, como estados "True" e "false" por exemplo.

## Formatação de texto

Os texto no HTML ficam entre as tags, existem algumas tag específicas para texto além de \<h1>... temos varias tags disponíveis:
- \<b> = Transforma o texto em <b>negrito</b>.
- \<i> = Transforma o texto em <i>itálico</i>.
- \<u> = Adiciona um <u>sublinhado</u> abaixo do texto.
- \<blockquote> = Serve para colocar espaçamento lateral no texto, e assim criar uma citação, fechando o texto e formato de bloco.
- \<sup> = Deixa qualquer caractere acima da paralavra anterior, exeplo: 10<sup>aqui esta o sup</sup>.
- \<sub> = Parecido com o sup, porém deixa a proxima palavra abaixo e menor que a anterior: 10<sub>aqui esta o sub</sub>.
- \<strong> = Também deixa em negrito, a diferença entre ele e o Bold, é por que o STRONG mostra ao navegador que aquela parte do texto é importante, e precisa ter uma ênfase, quando o bot de descrição for falar o texto para alguém.
- \<mark> = Deixa um marca-texto na <mark>palavra</mark>

### Definindo a Estrutura

Para estruturar uma página HTML precisamos entender como funciona a estrutura de uma página, ja sabemos que o HTML é a estrutura, e o CSS é o estilo, porém o CSS precisa saber exatamente em que ponto da página precisa ser modificado, para isso nossa estrutura precisa estar bem construída e identificada, para nos auxiliar nisso temos tags principais:

 - \<div> = Essa tag, cria uma limitação, ou seja, ela cria um bloco que contem tudo dentro dela, por padrão ela ocupa toda a horizontal do site, então ela faz um quebra de linha. Podemos imaginar a DIV como uma caixa onde colocamos todas as outras tags, e que podemos trabalhar somente nela pelo CSS.
 - \<span> = Essa tag assim como a div, cria um bloco, mas não ocupa toda a página, apenas o espaço que foi delimitado.
 - \<fieldset> = Essa tag segmenta uma área, a diferença entre ele e o DIV é que ele apresenta um linha, e possui uma tag chamada \<legend>, que cria uma legenda para aquele bloco em específico.
 - \<iframe> = Essa tag consegue exportar de outros site um recurso, ou uma página inteira, muito utilizado em google maps e videos de youtube por exemplo. 

### Tags de Mídias

As tags de mídia englobam todo tipo de mídia possível em uma página web, videos, imagens e audios. As mídias enriquecem a experiência do usuário, e cada uma tem seus parâmetro e peculiaridades
As mais utilizadas são:

- \<img> = Essa tag importa imagens ou GIF's, porém ela tem parâmetros para que não fique desproporcional ao conteúdo. Ela precisa da tag src="link da imagem" para funcioanar, mas também precisa ser definido o tamanho com width="" height="" para ficar dentro do padrão. Mais parâmetros podem ser encontrados na documentação.
- \<audio> = Essa tag Pai precisa de uma tag filho para funcionar que é semelhante ao parâmetro src="", porém é uma tag Filho chamada \<source src=""> com um parâmetro que identifica qual arquivo precisa ser aberto.
essa tag possui o atributo "controls" que ativa os controles de audios como "Play\Stop" e "Volume", sem o controls o player audio fica invisível.
- \<video> = Essa tag Pai precisa de uma tag filho chama <source> com uma parâmetro "src =""" para ele saber qual arquivo deve abrir, é importante que tenha dois formatos de vídeo, além do MP4 pode inserir na tag Pai, duas tags \<source> sendo uma MP4 e outra WebM por exemplo, assim se um navegador não funcionar MP4 ele tentará o Webm.
- \<track> = Essa tag possuí diversos parâmetros, mas em geral ela serve para adicionar legendas a vídeos, podendo ser em outros idiomas, além disso ela tem outros parâmetros relacionado a acessibilidade, ela é uma tag filho da \<video>, para legendas ele usa o formato .vtt, que é um formato texto para legendas.
- 

Não podemos esquecer da Acessibilidade, toda mídia precisa conter os dois parâmetros indispensáveis, Title="" e Alt="", essas tags descrevem para quem tem deficiência visual o que está sendo mostrado na tela.
Para testes pode ser utilizado o programa "NVDA" 

### Tabelas 
O conceito de tabelas no HTML é simples, para criar uma tabela precisamos criar uma espaço reservado para ela, um tag \<table> e dentro dela inserir linha e colunas, os dados serão identificados conforme suas tag's:

\<tr> = Table-Row - Define uma linha na tabela, ao inserir Table-Data dentro, ele colocará os dados lado a lado formando uma linha
\<td> = Table-data - Define o dado que vai nessa coluna/linha
\<th> = Table-Head - É o cabeçalho da tabela, define o nome de cada coluna. Como regra, o nome deve ser pequeno, para mais detalhes usa-se o atributo (title="")
\<thead> = Ele é usado apra agrupar as tags \<th> dentro, para melhor visualização do código.
\<tbody> = Ele agrupa todos as tags \<tr> dentro, para melhor vizualização do código. É o corpo principal da página
\<tfoot> = Ele agrupa \<tr> e \<td> referente ao fim da tabela, é o rodapé da nossa tabela.
\<caption> = Ele define o título principal, ficará acima do cabeçalho.

Para acessibilidade é interessante usar também na tag Table o atributo "sumary="Escreva a descrição detalhada da tabela", para mostrar para o leitor de tela exatamento do que se trata. 
