# Repetição e posicionamento da imagem de fundo

A propriedade `background-repeat` controla as repetições da imagem de fundo.

###### exemplos:

``` css
/*Repete a imagem apenas horizontalmente*/
body {
    background-image: url("img-01.jpg");
    background-repeat: repeat-x;
}
```

``` css
/*Repete a imagem apenas verticalmente*/
body {
    background-image: url("img-01.jpg");
    background-repeat: repeat-y;
}
```

``` css
/*Mostra a imagem de fundo apenas uma vez, sem repetições*/
body {
    background-image: url("img-01.jpg");
    background-repeat: no-repeat;
}
```

___

### Definindo a posição da imagem de fundo

A propriedade `background-position` define a posição da imagem de fundo.

###### exemplo:

```css
/*Posiciona a imagem de fundo no canto superior direito*/
body {
    background-image: url("img-01.jpg");
    background-position: right top;
}
```

***

> **PRÓXIMO AULA:** [Definindo uma imagem fixa ou com rolagem - Propriedade `background-attachment`](../3.4-background-attachment)

***


> **FONTE DO CONTEÚDO**:
>
> - [W3Schools - ]()
