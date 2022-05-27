# Definindo imagem fixa ou com rolagem

A propriedade `background-attachment` define se a imagem irá rolar junto com a página o se ele ficará fixa.

###### exemplo:

``` css
/*Define que a imagem de fundo seja fixa*/
body {
    background-image: url("img-01.jpg");
    background-repeat: no-repeat;
    background-position: right top;
    background-attachment: fixed;
}
```

``` css
/*Define que a imagem de fundo role junto com o conteúdo da página*/
body {
    background-image: url("img-01.jpg");
    background-repeat: no-repeat;
    background-position: right top;
    background-attachment: scroll;
}
```

***

> **PRÓXIMO AULA:** [Abreviando o código](../3.5-abreviacao)

***


> **FONTE DO CONTEÚDO**:
>
> - [W3Schools - ]()
