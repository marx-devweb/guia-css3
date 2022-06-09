# Flexbox

O **flexbox** nos permite criar um layout eficiente, alinhar e distribuir elementos na tela, mesmo se o tamanho desses elementos for dinâmico. A ideia principal da propriedade *flex* é ser flexível, permitindo alterar propriedades como altura, largura e ordem afim de se adaptar da melhor forma possível no espaço disponível, podendo se expandir ou diminuir de acordo com a necessidade prevenindo que o layout quebre. Com o Flexbox também é possível definir a direção e o posicionamento dos elementos verticalmente e horizontalmente

> **Nota:** O **flexbox** é mais apropriado para os componentes de um aplicativo e layouts de pequena escala, enquanto o layout de **grid** é destinado a layouts de maior escala.

### Conceitos básicos

O Flexbox é um modulo que possui várias propriedades, sendo que algumas delas são definidas no elemento "pai", enquanto outras são definidas no elemento "filho".

<img src="img-01.svg" style="width: 600px;" />

- **main axis** (eixo principal) - é onde são inseridos os itens, o eixo principal pode ser tanto vertical quanto horizontal, dependendo da propriedade definida no `flex-direction`.
- **main-start** | **main-end** (inicio | final) - os itens são dispostos no container a partir do inicio (main-start) em direção ao final (main-end).
- **main size** (tamanho principal) - a largura ou altura de um item dentro do container, sendo que a propriedade principal será definida pela direção vertical ou horizontal, podendo ser respectivamente a largura ou altura.
- **cross axis** (eixo transversal) - é o eixo perpendicular ao eixo principal e sua direção depende da do eixo principal.
- **cross-start** | **cross-end** (eixo inicial | eixo final) - flex lines que são preenchidas com itens e distribuídas iniciando pelo eixo inicial e indo em direção ao eixo final.
- **cross size** (tamanho do eixo) - será a largura ou altura de um item dentro do container, dependendo de qual é sua direção.

## Propriedades do Flexbox

Como já foi dito anteriormente algumas das propriedades serão definidas no **elemento pai** enquanto outras serão definidas no **elemento filho**.

O elemento pai é o contêiner que vai englobar todos os itens e é nele que será definido o `display`: `flex` e também outras propriedades de posicionamento e alinhamento. E o elemento filho são justamente os itens dentro do contêiner. 

O código HTML abaixo exemplifica uma estrutura básica:

```html
<!--Aqui definimos um contêiner flexível com 3 itens flexíveis-->
<div class="container"><!--container-->
  <div>item 1</div><!--item 1-->
  <div>item 2</div><!--item 2-->
  <div>item 3</div><!--item 3-->
</div>
```

#### Propriedades definidas no elemento pai (contêiner flexível):

- [`display`](01-propriedades-elemento-pai)
- [`flex-direction`](01-propriedades-elemento-pai)
- [`flex-wrap`](01-propriedades-elemento-pai)
- [`flex-flow`](01-propriedades-elemento-pai)
- [`justify-content`](01-propriedades-elemento-pai)
- [`align-items`](01-propriedades-elemento-pai)
- [`align-content`](01-propriedades-elemento-pai)

#### Propriedades definidas no elemento filho (itens flexíveis):

- [`order`](02-propriedades-elemento-filho)
- [`flex-grow`](02-propriedades-elemento-filho)
- [`flex-shrink`](02-propriedades-elemento-filho)
- [`flex-basis`](02-propriedades-elemento-filho)
- [`flex`](02-propriedades-elemento-filho)
- [`align-self`](02-propriedades-elemento-filho)

***

#### FONTE DO CONTEÚDO:

- [W3Schools - Flexbox](https://www.w3schools.com/css/css3_flexbox.asp)

- [CSS TRICKS - Um guia completo para Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
