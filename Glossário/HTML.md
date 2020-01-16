### O Que é HTML?

HTML significa Hypertext Markup Language. Ele permite que os usuários criem e estruturem seções, parágrafos, cabeçalhos e links para páginas da internet ou aplicações.

O HTML não é uma linguagem de programação, isso significa que não pode ser usado para criar funcionalidades dinâmicas. Entretanto, o HTML possibilita a organização e formatação de documentos, similar ao Microsoft Word.

Ao trabalhar com HTML simplesmente codificamos estruturas (tags e atributos) para marcar a página de um site. Por exemplo, podemos criar um parágrafo colocando o texto entre as tags **<p>** e **</p>**.

### Como o HTML Funciona?

Documentos HTML são arquivos com as extensões .html ou .htm. Eles podem ser visualizados com qualquer navegador (como Google Chrome, Safari, ou Mozilla Firefox). O navegador faz a leitura do arquivo e renderiza seu conteúdo para visualização dos usuários.

Cada página HTML consiste em uma série de tags (também chamadas de elementos), que podem ser consideradas os blocos de construção das páginas. Elas criam uma hierarquia que estrutura o conteúdo entre seções, parágrafos, cabeçalhos e outros blocos de conteúdo.

A maioria dos elementos HTML utilizam as sintaxe de abertura e fechamento como **<tag>** e **</tag>**.

### Revisão das Tags HTML mais Utilizadas

As HTML tags possuem dois tipos principais: elementos bloco e elementos em linha.

#### Elementos bloco 

Utilizam todo o espaço disponível e começam uma nova linha no documento. Cabeçalhos e parágrafos são bons exemplos de elementos bloco. Os três elementos bloco que todo documento HTML precisa conter são **<html>**, **<head>**, e **<body>**.

- A tag **<html></html>** é o elemento de maior nível que está em todas as páginas HTML.
- A tag **<head></head>** possui informações do meta como o título e charset da página.
- A tag **<body></body>** engloba todos os elementos que são mostrados na página.

Os cabeçalhos possuem 6 níveis no HTML. Eles englobam desde **<h1></h1>** até **<h6></h6>**, onde o h1 é o maior nível e h6 o menor. Parágrafos possuem as tags <p></p>, enquanto os blockquotes (ou elementos HTML de citação de blocos) utilizam a tag **<blockquote></blockquote>**.

Divisões são seções de conteúdo maiores que geralmente possuem parágrafos, imagens, de vez em quando blockquotes, e outros elementos menores. Podemos marcá-los com as tags **<div></div>**. Um elemento div pode conter outro elemento div dentro.

Você também pode utilizar as tags **<ol></ol>** para listas ordenadas e **<ul></ul>** para desordenadas. Itens individuais da lista devem conter as tags **<li></li>**. 

#### Elementos em linha 

Utilizam apenas o espaço necessário e não criar uma quebra de linha. Eles geralmente são utilizados para formatar os elementos dentro de um elemento bloco. Links e strings enfatizadas são bons exemplos de elementos em linha.

Muitos elementos em linhas são utilizados na formatação de textos. Por exemplo, uma tag **<strong></strong>** renderiza um elemento em negrito, enquanto as tags **<em></em>** mostram em itálico.

Hyperlinks também são elementos em linha que utilizam as tags **<a></a>** e o atributo href para indicar a destinação do link

### A Evolução do HTML. Qual a diferença entre HTML e HTML5?

Um dos mais aguardados é a incorporação nativa de vídeos e arquivos de áudios. Ao invés de precisar utilizar o Flash Player, agora é possível incorporar vídeos e áudios com as novas tags **<audio></audio>** e **<video></video>**. Ele também possui compatibilidade com SVG (vetor gráfico escalável) e MathML para fórmulas científicas e matemáticas.

O HTML5 também introduziu algumas melhorias de semântica. As novas tags semânticas informam ao navegador sobre o significado do conteúdo, o que auxilia tanto os leitores quanto os mecanismos de busca.

As tags semânticas mais populares são **<article></article>**, **<section></section>**, **<aside></aside>**, **<header></header>**, e **<footer></footer>**.

### Qual a Relação Entre HTML, CSS e JavaScript?

O CSS é responsável pelo estilo como background, cores, layouts, espaçamentos, e animações.
JavaScript permite a adição de funcionalidades dinâmicas como sliders, pop-ups, e galerias de fotos.