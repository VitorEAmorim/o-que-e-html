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
