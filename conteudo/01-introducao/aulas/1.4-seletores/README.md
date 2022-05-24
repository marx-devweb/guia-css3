# Seletores

Um seletor CSS é a primeira parte de uma regra CSS. Ele informa o navegador quais elementos HTML deve ser selecionado para que os valores das propriedades CSS sejam aplicados a eles, ou seja, ele selecionam os elementos HTML a serem estilizados.

---

### Lista de seletores

Quando possuímos mais de um elemento que possui a mesma formatação CSS com seletores individuais, podemos combina-lós em uma *lista de seletores* para que a regra seja aplicada a todos os seletores individuais.

No exemplo abaixo, temos 2 regras CSS, uma para o elemento `h1` e uma para a classe `.special`:

```css
h1 {
  color: blue;
}

.special {
  color: blue;
}
```

Podemos combina-lós em uma lista de seletores, adicionando uma vírgula entre eles.

```css
h1, .special {
  color: blue;
}
```

Quando agrupamos seletores dessa forma, se algum seletor for inválido, toda a regra será ignorada.

---

### Tipos de seletores

Existem alguns grupos diferentes de seletores:

#### Seletores de tipo

Este seletor as vezes é chamado de seletor de *nome de tag* ou seletor de *elemento*, pois seleciona uma tag/elemento HTML no documento.

No exemplo abaixo, utilizamos os seletores `span`, `em` e `strong`:

```css
span {
    background-color: yellow;
}

strong {
    color: rebeccapurple;
}

em {
    color: rebeccapurple;
}
```

<br>

#### Seletor universal

Este seletor é indicado por um asterisco (`*`). Ele seleciona tudo dentro do documento (ou dentro do elemento pai se estiver sendo encadeado com outro elemento e um combinador descendente). 

No exemplo abaixo, o seletor universal remove as margens de todos os elementos.

```css
* {
    margin: 0;
}
```

<br>



















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
