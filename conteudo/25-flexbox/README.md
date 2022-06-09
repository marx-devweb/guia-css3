# Layout Flexbox

O layout Flexbox torna mais fácil projetar uma estrutura de layout responsiva flexível sem usar flutuação ou posicionamento, ele visa fornecer uma maneira mais eficiente de dispor, alinhar e distribuir o espaço entre os itens em um contêiner, mesmo quando seu tamanho é desconhecido e/ou dinâmico.

A principal ideia do layout Flexbox é dar ao contêiner a capacidade de alterar a largura/altura e a ordem de seus itens para preencher melhor o espaço disponível, principalmente para acomodar todos os tipos de dispositivos de exibição e tamanhos de tela. 

> **Nota:** O layout Flexbox é mais apropriado para os componentes de um aplicativo e layouts de pequena escala, enquanto o layout de **Grid** é destinado a layouts de maior escala.

#### Características do Flexbox

- Centralizar um bloco de conteúdo verticalmente dentro do elemento pai.
- Fazer com que os elementos filhos de um container ocupe uma quantidade igual de largura/altura disponível, independente da quantidade de largura/altura disponível.
- Fazer todas as colunas de um layout com múltiplas colunas adotem a mesma altura, mesmo que contenham uma quantidade diferente de conteúdo.

---

### Definindo um contêiner flexível 

Para começar a usar o modelo Flexbox, definiremos um contêiner flexível. 

###### exemplo:

```html
<!--Aqui definimos um container flexível com 3 itens flexíveis-->
<div class="container"><!--container-->
  <div>item 1</div><!--item 1-->
  <div>item 2</div><!--item 2-->
  <div>item 3</div><!--item 3-->
</div>
```



#### Propriedades CSS para um contêiner flexível:

- `flex-direction`
- `flex-wrap`
- `flex-flow`
- `justify-content`
- `align-items`
- `align-content`







As propriedades para itens flexíveis (elemento filho) são:

- [`order`]()
- [`flex-grow`]()
- [`flex-shrink`](k)
- [`flex-basis`]()
- [`flex`]()
- [`align-self`]()



###### exemplo:





###### exemplo:





###### exemplo:





###### exemplo:

#### Assuntos abordados: 



1. [Definindo um container](aulas/25.2-container)
2. [Definindo itens](aulas/25.3-itens)
3. [Flex responsivo](aulas/25.4-responsive)
