# Cores RGB

>  RGB representa fontes de luz VERMELHA, VERDE e AZUL.

Formula para cores RGB:

`rgb (red, green, blue)`

Cada parâmetro (vermelho, verde e azul) define a intensidade da cor com um valor entre 0 e 255.

###### exemplos:

````html
<h1 style="background-color:rgb(255, 0, 0);">rgb(255, 0, 0)</h1>
<h1 style="background-color:rgb(0, 0, 255);">rgb(0, 0, 255)</h1>
<h1 style="background-color:rgb(60, 179, 113);">rgb(60, 179, 113)</h1>
<h1 style="background-color:rgb(238, 130, 238);">rgb(238, 130, 238)</h1>
<h1 style="background-color:rgb(255, 165, 0);">rgb(255, 165, 0)</h1>
<h1 style="background-color:rgb(106, 90, 205);">rgb(106, 90, 205)</h1>
````

---

### Tons de cinza

Para definir tons de cinza, geralmente devemos utilizar valores iguais para todos os três parâmetros.

###### exemplos:

``` html
<h1 style="background-color:rgb(60, 60, 60);">rgb(60, 60, 60)</h1>
<h1 style="background-color:rgb(100, 100, 100);">rgb(100, 100, 100)</h1>
<h1 style="background-color:rgb(140, 140, 140);">rgb(140, 140, 140)</h1>
<h1 style="background-color:rgb(180, 180, 180);">rgb(180, 180, 180)</h1>
<h1 style="background-color:rgb(200, 200, 200);">rgb(200, 200, 200)</h1>
```

---

### Valor RGBA

Os valores de cor RGBA são uma extensão dos valores de cor RGB com um canal alfa - que especifica a opacidade de uma cor.

Formula para cores RGBA:

`rgba( red, green, blue, alfa)`

O parâmetro alfa é um número entre 0,0 (totalmente transparente) e 1,0 (nada transparente):

``` html
<h1 style="background-color:rgba(255, 99, 71, 0);">rgba(255, 99, 71, 0)</h1>
<h1 style="background-color:rgba(255, 99, 71, 0.2);">rgba(255, 99, 71, 0.2)</h1>
<h1 style="background-color:rgba(255, 99, 71, 0.4);">rgba(255, 99, 71, 0.4)</h1>
<h1 style="background-color:rgba(255, 99, 71, 0.6);">rgba(255, 99, 71, 0.6)</h1>
<h1 style="background-color:rgba(255, 99, 71, 0.8);">rgba(255, 99, 71, 0.8)</h1>
<h1 style="background-color:rgba(255, 99, 71, 1);">rgba(255, 99, 71, 1)</h1>
```

***

> **PRÓXIMO AULA:** [Cores HEX](../2.3-cores-hex)

***


> **FONTE DO CONTEÚDO**:
>
> - [W3Schools - Cores RGB](https://www.w3schools.com/css/css_colors_rgb.asp)
