# Seletores

Um seletor CSS é a primeira parte de uma regra CSS. Ele seleciona os elementos HTML que serão estilizados.

### Seletor de elementos

Selecionas os elementos HTML pelo nome do elemento.

###### Exemplo:

```css
p {
    text-aling: center;
    color: red;
}
```

---

### Agrupamento de seletores 

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

Podemos agrupa-los em uma lista de seletores separando cada seletor com uma vírgula:

```css
h1, h2, p {
  text-align: center;
  color: red;
}
```

---

### Seletor universal

Seleciona todos os elementos HTML de uma página. Ele e indicado por um (`*`).

No abaixo, o seletor universal remove as margens da página.

```css
* {
    margin: 0;
}
```

---

### Seletor de class

Seleciona os elementos HTML com um atributo de class específico. 

Este seletor é declarado com um caractere `.` seguido pelo nome da class. 

No exemplo abaixo, todos os elementos com a `class="destaque"` receberam a estilização:

```html
<body>
    <h1>Seletor de Classe</h1>
    <p>Veggies es bonus vobis, proinde vos postulo essum magis <span class="destaque">kohlrabi welsh onion</span> daikon amaranth tatsoi tomatillo melon azuki bean garlic.
    </p>
    <p class="destaque">Gumbo beet greens corn soko <strong>endive</strong> gumbo gourd. Parsley shallot courgette tatsoi pea sprouts fava bean collard greens dandelion okra wakame tomato. Dandelion cucumber earthnut pea peanut soko zucchini.
    </p>
</body>
```

```css
.destaque {
    background-color: yellow
}
```

Também podemos criar regras CSS individuais para elementos com a mesma class aplicada.

No código HTML abaixo, o cabeçalho `<h1>` e o elemento `<span>` possui a mesma `class="destaque"` aplicada.

```html
...
<body>
    <h1 class="destaque">Seletor de Classe</h1>
    <p>Veggies es bonus vobis, proinde vos postulo essum magis <span class="destaque">kohlrabi welsh onion</span> daikon amaranth tatsoi tomatillo melon azuki bean garlic.
    </p>    
</body>
...
```

Mesmo com a mesma `class="destaque"` aplicada, vamos estilizar `<h1>` e `<span>` com backgrounds de cor diferentes. Fazemos isso usando o seletor de tipo para o elemento que queremos direcionar, com a classe anexada usando um ponto, sem espaço em branco no meio.

```css
h1.destaque{
    background-color:yellow;
}

span.destaque{
    bacground-color:blue;
    color:white;
}
```

<br>

#### Seletores de ID

Este seletor começa com o caractere (`#`). 





















#### Seletores de tipo, classe e ID

Selecionam elementos HTML, como um `<h1>`:

``` css
h1 { }
```

Selecionam classe:

``` css
.box { }
```

É também ID:

``` css
#unique { }
```

<br>

#### Seletores de atributos:

Este grupo de seletores oferece diferentes maneiras de selecionar elementos com base na presença de um determinado atributo em um elemento:

``` css
a[title] { }
```

Ou ainda fazer uma seleção com base na presença de um atributo com um determinado valor:

``` css
a[href="https://example.com"] { }
```

<br>

#### Seletores de pseudo-classes

Este seletor estiliza certos estados de um elemento. Por exemplo, a pseudo-classe `:hover`, seleciona um elemento apenas quando ele está sendo passado pelo ponteiro do mouse:

```css
a:hover { }
```

<br>

#### Seletores de pseudo-elementos

Este seletor selecionam uma determinada parte de um elemento em vez do próprio elemento. Por exemplo, `::first-line` sempre seleciona a primeira linha de texto dentro de um determinado elemento.

```css
p::first-line { }
```

<br>

#### Seletores combinadores

Este grupo de seletores combina outros seletores para direcionar elementos em nossos documentos. No exemplo abaixo, o seletor seleciona parágrafos que são filhos diretos de elementos `<article>` usando o combinador filho (`>`):

``` css
article > p { }
```





***

> **PRÓXIMO AULA:** [Como adicionar CSS3](../1.5-como-adicionar-css)

***


> **FONTE DO CONTEÚDO**:
>
> - [W3Schools - Seletores CSS](https://www.w3schools.com/css/css_selectors.asp)
> - [MDN - Seletores CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors)
