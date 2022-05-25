# Seletores

Um seletor CSS é a primeira parte de uma regra CSS. Ele seleciona os elementos HTML que serão estilizados.

### Seletores de elementos

Selecionas os elementos HTML pelo nome do elemento.

###### Exemplo:

```css
h2 {
    background-color: blue;
    color: white;
}

p {
    text-aling: center;
    color: red;
}

span {
    background-color: yellow;
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

Para agrupa-los em uma lista de seletores, separamos cada seletor com uma vírgula:

```css
h1, h2, p {
  text-align: center;
  color: red;
}
```

---

### Seletor universal

Seleciona todos os elementos HTML de uma página. Ele e indicado por um (`*`).

O exemplo abaixo, remove as margens da página.

```css
* {
    margin: 0;
}
```

---

### Seletor de classe

Seleciona os elementos HTML com um atributo de class específico. 

Este seletor é declarado com um caractere `.` seguido pelo nome da class. 

###### exemplo:

```css
.destaque {
    background-color: yellow
}
```

Também podemos definir quais elementos HTML que possuem a mesma class receba a definição de estilo.

No código HTML abaixo, os elementos `<h1>` e  `<span>` possui a mesma `class="destaque"`.

```html
...
<body>
    <h1 class="destaque">Seletor de Classe</h1>
    <p>Veggies es bonus vobis, proinde vos postulo essum magis <span class="destaque">kohlrabi welsh onion</span> daikon amaranth tatsoi tomatillo melon azuki bean garlic.
    </p>    
</body>
...
```

Vamos estilizar `<h1>` e `<span>` com backgrounds de cor diferentes. 

Fazemos isso usando o seletor de tipo para o elemento que queremos direcionar, com a classe anexada usando um ponto, sem espaço em branco no meio.

```css
h1.destaque{
    background-color:yellow;
}

span.destaque{
    bacground-color:blue;
    color:white;
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

---

### Seletores de ID

Seleciona um elemento HTML com um atributo de id específico. 

Ele é utilizado da mesma maneira que um seletor de class. No entanto, este seletor so pode ser usado uma vez por página, e os elementos só podem ter um único lavor `id` aplicado.  

Este seletor começa com o caractere `#` seguido pelo nome do elemento `id`.

###### exemplo:

```css
#container {
    width:720px;
    heigth: 300px;    
    background-color: blue;
    color:white;
}
```

***

> **PRÓXIMO AULA:** [Como adicionar CSS3](../1.5-como-adicionar-css)

***


> **FONTE DO CONTEÚDO**:
>
> - [W3Schools - Seletores CSS](https://www.w3schools.com/css/css_selectors.asp)
> - [MDN - Seletores CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors)
