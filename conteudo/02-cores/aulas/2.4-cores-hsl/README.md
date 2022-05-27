# Cores HSL

hsl (*matiz* , *saturação* , *luminosidade*)

- Matiz é um grau na roda de cores de 0 a 360. 0 é vermelho, 120 é verde e 240 é azul.

- Saturação é um valor percentual, 0% significa um tom de cinza e 100% é a cor completa.

- Luminosidade também é um valor percentual, 0% é preto e 100% é branco.

###### exemplos:

```` html
<h2 style="background-color:hsl(0, 100%, 50%);">Vermelho</h2>
<h2 style="background-color:hsl(240, 100%, 50%);">Azul</h2>
<h2 style="background-color:hsl(147, 50%, 47%);">Verde</h2>
````

---

### Saturação

A saturação pode ser descrita como a intensidade de uma cor, onde 100% é cor pura, sem tons de cinza, 50% é 50% cinza, mas você ainda podemos ver a cor é 0% é completamente cinza, onde não podemos mais ver a cor.

``` html
<h2 style="background-color:hsl(0, 100%, 50%);">Cor pura</h2>
<h2 style="background-color:hsl(0, 50%, 50%);">50% de saturação</h2>
<h2 style="background-color:hsl(0, 0%, 50%);">Totalmente saturado</h2>
```

---

### Luminosidade

A leveza ou luminosidade e quantidade de luz na cor, onde 0% significa sem luz (preto), 50% significa 50% luz (nem escuro nem claro) 100% significa luminosidade total (branco).

``` html
<h2 style="background-color:hsl(0, 100%, 0%);">Cor sem luminosidade</h2>
<h2 style="background-color:hsl(0, 100%, 25%);">Cor com 25% de luminosidade</h2>
<h2 style="background-color:hsl(0, 100%, 50%);">Cor com 50% de luminosidade</h2>
```

---

### Tons de cinza

Os tons de cinza são definidos com a matiz e a saturação com 0 e ajustando a luminosidade de 0% a 100% para obter tons mais escuros/mais claros.

``` html
<h2 style="background-color:hsl(0, 0%, 20%);">20% de luminosidade</h2>
<h2 style="background-color:hsl(0, 0%, 60%);">60% de luminosidade</h2>
<h2 style="background-color:hsl(0, 0%, 80%);">80% de luminosidade</h2>
```

---

### Valores de cores HSLA

Os valores de uma cor HSLA, simplesmente são os valores das cores HSL mais um canal Alfa - que especifica a opacidade de uma cor.

hsla (*matiz,* *saturação* , *luminosidade, alfa* )

O parâmetro alfa é um número entre 0,0 (totalmente transparente) e 1,0 (nada transparente):

``` html
<h2 style="background-color:hsla(9, 100%, 64%, 0);">Cor sem opacidade</h2>
<h2 style="background-color:hsla(9, 100%, 64%, 0.2);">Cor com 0.2 de opacidade</h2>
<h2 style="background-color:hsla(9, 100%, 64%, 0.4);">Cor com 0.4 de opacidade</h2>
```

***

> **PRÓXIMO TEMA:** [Definindo planos de fundo - **Propriedade `background`**](/conteudo/03-backgrounds)

***


> **FONTE DO CONTEÚDO**:
>
> - [W3Schools - Cores HSL e HSLA](https://www.w3schools.com/css/css_colors_hsl.asp)
