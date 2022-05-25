# CSS3

### Introdução

CSS é uma linguagem para estilizar páginas da web.

- CSS significa Cascading Style Sheets;
- CSS economiza muito trabalho. Ele pode controlar o layout de várias páginas da web de uma só vez

CSS pode ser usado para estilizar um documento muito básico de texto, por exemplo, alterar a cor e tamanho dos títulos e links. Pode ser usado para criar layout e efeitos tais como animações.

---

### Sintaxe

CSS é uma linguagem baseada em regras. 

O exemplo abaixo mostra uma regra CSS muito simples:

![](F:\guia-css3\conteudo\01-introducao\img_selector.gif)

- `h1` é o seletor que define o elemento HTML a ser estilizado;
- Em seguida temos um conjunto de chaves `{ }`. Dentro conjunto temos duas declarações, separadas por ponto e vírgula. 
- Ambas as declarações são compostas por propriedades e valores. No exemplo `color` é a propriedade e `red` o valor;

---

### Seletores CSS

Um seletor CSS é a primeira parte de uma regra CSS. Ele seleciona os elementos HTML que serão estilizados. 

Abaixo os seletores mais báscos. 

#### Seletores de elementos

Selecionas os elementos HTML pelo nome do elemento.

###### sintaxe: 

```css
elemento {
    propriedade: valor;
}
```

###### exemplo:

```css
h2 {
    background-color: blue;
}
```

<br>

#### Seletores de ID

Seleciona um elemento HTML com um atributo de id específico. 

Cada seletor de `id` só pode ser utilizado uma vez na pagina.

###### sintaxe:

```css
#nome_id {
    propriedade: valor;
}
```

###### exemplo:

```css
#container {
    width:720px;
    heigth: 300px;    
}
```

<br>

#### Seletor de classe

Seleciona os elementos HTML com um atributo de class específico. 

Cade seletor de classe pode ser utilizado em mais de um elemento HTML.

###### sintaxe:

```css
.nome_class {
    propriedade: valor;
}
```

###### exemplo:

```css
.destaque {
    background-color: yellow
}
```

Também podemos definir quais elementos HTML que possuem a mesma class receba a definição de estilo.

No código HTML abaixo, os elementos `<h1>` e  `<span>` possuem a mesma `class="destaque"`.

```html
...
<body>
    <h1 class="destaque">Seletor de Classe</h1>
    <p>O seletor de classes CSS corresponde aos <span class="destaque">elementos</span> com base no conteúdo de seus atributos class.</p>    
</body>
...
```

Vamos estilizar `<h1>` e `<span>` com backgrounds de cor diferentes. 

```css
h1.destaque{
    background-color:yellow;
}

span.destaque{
    background-color:blue;
}
```

**Os elementos HTML também pode receber mais de uma class.**

###### código HTML:

```html
<p class="texto-centralizado texto-grande">Este paragrafo esta centralizado e tem um tamanho de 30px.</p>
```

###### código CSS:

```css
.texto-centralizado{
    text-aling: center;
}

.texto-grande{
    font-size:30px
}
```

<br>

#### Seletor universal

Seleciona todos os elementos HTML de uma página.

###### sintaxe:

```css
* {
    propriedade: valor;
}
```

###### O exemplo abaixo, remove as margens da página.

```css
* {
    margin: 0;
}
```

<br>

#### Seletore de agrupamento

Seleciona todos os elementos HTML com as mesma definições de estilo.

No exemplo abaixo, os elementos `h1`, `h2` e `p` possui as mesma definições de estilo:

```css
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```

Para agrupa-los em uma lista de seletores, separamos cada seletor com uma vírgula:

```css
h1, h2, p {
  text-align: center;
  color: red;
}
```

---

### Como adicionar CSS

Existem 3 maneiras de inserir uma folha de estilo na nossa página:

#### CSS externo

Para vincular uma folha de estilos externa no nosso documento HTML, devemos salvar um aquivo com a extensão `.css` e depois um elemento `<link>`, na seção `<head>`, conforme exemplo abaixo:

```css
<link rel="stylesheet" href="style.css">
```

<br>

#### CSS interno

Este tipo de folha de estilo deve ser declarada dentro do elemento `<style>` na seção `<head>`, conforme o exemplo abaixo:

```html
<head>
    <style>
        body {
            background-color: linen;
        }
        h1 {
            color: maroon;
            margin-left: 40px;
        }
    </style>
</head>
```

<br>

### CSS inline

É usado para estilizar um elemento HTML específico. 

Para utilizar o css inline, devemos adicionar o atributo **style** no elemento que queremos estilizar, conforme exemplo abaixo:

```html
<body>
    <h1 style="color:blue;text-align:center;">Este é um cabeçalho</h1>
    <p style="color:red;">Este é um parágrafo.</p>
</body>
```

---

### Cometários

Os comentários começa com `/*` e termina com `*/`.

###### exemplo:

```css
/*Este é um comentário de uma linha*/
p {
  color: red;
}
```

***

> **PRÓXIMO TEMA:** [Definindo Cores](/conteudo/02-cores)

***


> **FONTE DO CONTEÚDO**:
>
> - [W3Schools - Introdução](https://www.w3schools.com/css/css_intro.asp)
> - [W3Schools - Sintaxe](https://www.w3schools.com/css/css_syntax.asp)
> - [W3Schools - Seletores](https://www.w3schools.com/css/css_selectors.asp)
> - [W3Schools - Como adicionar CSS](https://www.w3schools.com/css/css_howto.asp)
> - [W3Schools - Comentários](https://www.w3schools.com/css/css_comments.asp)
