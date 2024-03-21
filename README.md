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

