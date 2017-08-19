# Documentação Regras CSS

## Grids

#### full div
Usar a classe "center" em todos os elementos que terão o width de 100%.
#### left e right div's
Usado para criar blocos com posições paralelas e width de 50% em relação a classe pai. 
>As posições já recebem por padrão a propriedade de "float" do respectivo nome da classe.

**exemplo:**
``` html
    <div class="center">
        <div class="left"></div>
        <div class="right"></div>
    </div> 
```
#### half div
Box usado para elementos com width padrão de 600px, ficando alinhado ao centro da div pai. Ficando chumbada a classe "center" como pai. 
>_Posição criada para suprir a nescessidade de mini banners centralizados._ 

**exemplo:**
```html
    <div class="center">
        <div class="half"></div>
    </div>
```

## Elementos padrão

#### Título
Título padrão.
**exemplo:**
```html
    <h1 class="title">example title text</h1>
```
#### Texto
Texto padrão.
**exemplo:**
```html
    <p class="text t-center">example text with align</p>
```
#### Link
Links estao esperando duas situações:
+ links em meio ao texto
 ```html
    <a href="#mylink" class="t-link">my link</a>
 ```
 + links geral
 ```html
    <a href="#mylink" class="link">general link</a>               
 ```
 ### Menu Interativo
 Os menus interativos receberam em seus links o Id dos elementos que eles vão indicar.
 **exemplo:**
 ```html
    <div class="i-menu">
        <div class=""><a href="#id1">content i-menu</a></div>
        <div class=""><a href="#id2">content i-menu</a></div>
        <div class=""><a href="#id3">content i-menu</a></div>
        <div class=""><a href="#id4">content i-menu</a></div>
    </div>
 ```
 ### Banner
Os banners estao esperando 3 sitações que descreveremos detalhadamente nos exemplos, entretando todas situações de banners compartilham como estrutura comum estar chumbado a classe "center" para facilitar o posicionamento.
 + Banner simples
 ```html
     <div class="center banner">
        <img src="/path/banner.jpg" alt="banner sample">
    </div>
 ```
 + Banner com descrição
 ```html
     <div class="center banner">
        <img src="/path/banner.jpg" alt="banner sample">
        <p class="banner-description text">example text with align</p>
    </div>
 ```
 + Banner com texto
 ```html
    <div class="center banner-text">
        <img src="/path/banner.jpg" alt="banner sample">
        <div class="background-text">
            <h1 class="title">example banner title</h1>        
            <p class="text">example banner text with align</p>   
        </div>
    </div>   
 ```
 #### Shelf's
 
As shelfs estão esperando duas situações de apresentação dos produtos, como Lista ou Slides.
Os produtos derveram ser setados dentro do campo "**data-sku**" separados por espaços da seguinte forma ``` data-sku="sku1 sku2 sku3 sku4" ```
+ Shelf List
```html
    <div class="center shelf-article shelf-list" data-sku="sku1 sku2 sku3"></div>
```
+ Shelf Slider
```html
    <div class="center shelf-article shelf-slider" data-sku="sku sku2 sku3"></div>
```
## Classes Disponíveis

**.center** classe para posicionamento 100% em relação a classe pai.
**.left/.right** classes para posionamento 50% em relação a div pai, sendo que left possui ``` float:left ``` e assim respectivamente.
**.half** classe criada para posicionamento de mini banners centralizados, possui ``` width:600px ``` e alinhamento centralizado.
**.t-left/.t-right/.t-center** classes para alinhamento de texto, adicionando a propriedade ` text-align ` com o sufixo da classe.
**.b-top/.b-bottom/.b-left/.b-right** classes para adição de borda ao elemento, sera adicionado ` border-left ` caso use a classe **t-left** e assim respectivamente.
**.title** classe para elementos de titulos, adiciona `text-transform: uppercase` e `font-size: 19px` 
**.text** classe para paragrafos, adiciona `font-size: 14px` e `margin: 0`
**.t-link** classe adicionada a links que estejam contidos em paragrafos, recebem a mesma formatação da classe **.text** com a adição da propriedade ` text-decoration: underline `.
**.link** classe usada para links de modo geral, segue o padrão de formatação da classe **.title**.
**.description-list** classe para listas na seguinte estrutura `ul>li`.
**.banner-text** classe para banner com caixa de texto.
**.background-text** classe que prepara o box de texto dos banner, sendo obrigado a ter como pai a classe **.banner-text**.
**.banner-slider** classe que prepara os controles do plugin _bx-slider_.
**.i-menu** classe que prepara o menu interativo, uma vez que o menu respeita a estrutura imposta neste documento.
**.shelf-article** classe esperada em toda shelf, alinha elementos dentro da shelf.
**.shelf-slider** classe esperada em shelf que tenham slider, ela prepara os controles para o _bx-slider_.