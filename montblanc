# Mont Blanc


![MacDown logo](http://i-montblancmx-dev.a8e.net.br/images/logo-mont-blanc-documentation.png)

Documentação Base par o Projeto **Mont Blanc**.

## StoreID

 - montblancmx


## Banners Desktop


### Menu

 - Banner Menu
    - Posição: Banner Menu
    - Template: Home Banner Menu
    - Tamanho: 262 x 276
    - Observações (obrigatório): Utilizar palavra-chave igual à classname do menu (ex: perfume)

### Home

 - Home Slider
    - Posição: Home Banner Principal
    - Template: Banner principal topo da página
    - Tamanho: 1200 x 460

 - Banner Destaque Home 1 (Pré Shelf)
    - Posição: Home Banner Destaques
    - Template: Banner Template com Texto
    - Tamanho: 590 x 350
    - Observações (opcional): Para ordenar os banners use o campo 'prioridade' utilizando números em ordem crescente

 - Banner Destaque Home 2 (Pós Shelf)
    - Posição: Home Banner Central
    - Template: Banner Template com Texto
    - Tamanho: 590 x 350
    - Observações (opcional): Para ordenar os banners use o campo 'prioridade' utilizando números em ordem crescente

 - Banner Home Bottom
    - Posição: Home Banner Destaque Footer
    - Template: Banner Template com Texto
    - Tamanho: 385 x 385
    - Observações (opcional): Para ordenar os banners use o campo 'prioridade' utilizando números em ordem crescente

### Departamento

 - Banner Departamento
    - Posição: Banner Principal Departamento
    - Template: Banner topo com titulo
    - Tamanho: 1200 x 200
    - Observações (obrigatório): É necessário escolher o departamento que deseja exibir o banner, na opção ‘Categorias do Banner’

 - Departamento Descricao
    - Posição: Banner Departamento Descricao
    - Template: Departamento Descrição

### Categoria

 - Banner Categoria
    - Posição: Banner Principal de Categoria
    - Template: Banner topo com titulo
    - Tamanho: 1200 x 200
    - Observações (obrigatório): É necessário escolher a categoria que deseja exibir o banner, na opção ‘Categorias do Banner’

## Banners Mobile

### Home

 - Mobile Home Slider
    - Posição: Home Mobile - Banner Principal
    - Template: Banner Mobile Home Principal
    - Tamanho (large): 1100 x 280
    - Tamanho (medium): 640 x 270
    - Tamanho (small): 380 x 280

 - Mobile Banner Destaque Home 1 (Pré Shelf)
    - Posição: Home Mobile - Banner Secundario
    - Template: Banner Template com Texto
    - Observações (opcional): Para ordenar os banners use o campo 'prioridade' utilizando números em ordem crescente

 - Mobile Banner Destaque Home 2 (Pós Shelf)
    - Posição: Home Mobile - Banner Central
    - Template: Banner Template com Texto
    - Observações (opcional): Para ordenar os banners use o campo 'prioridade' utilizando números em ordem crescente

 - Mobile Banner Home Bottom
    - Posição: Home Mobile - Banner Footer
    - Template: Banner Template com Texto
    - Observações (opcional): Para ordenar os banners use o campo 'prioridade' utilizando números em ordem crescente

### Departamento

 - Mobile Banner Departamento
    - Posição: Mobile  Banner Departamento
    - Template: Mobile Categoria/departamento
    - Observações (obrigatório): É necessário escolher o departamento que deseja exibir o banner, na opção ‘Categorias do Banner’

### Categoria

 - Mobile Banner Categoria
    - Posição: Mobile Banner Categoria
    - Template: Mobile Categoria/departamento
    - Observações (obrigatório): É necessário escolher a categoria que deseja exibir o banner, na opção ‘Categorias do Banner’

### Customizaçao de produto (Engraving / Embossing)


#### Requerimentos

##### SKUS

Skus necessários (cadastro no admin). 


|	SKU ID	|	Nome da Custom		|	 
|---|---								|
|110512|	Customization Text   	|
|110514|	Customization Typeface	|
|110513|	Customization Type   	|
|110515|	Engraving Position		|
|110516|	Embossing Color			|


Obs: Os skus precisam ser do tipo CTM, `visible: N` e todos os skus precisam estar produzidos, com preço e estoque. Para mais detalhes, clique [Leia a documentação aqui](https://lab.accurate.com.br/twiki/bin/view/Main/AcecFunctionalSpecificationsCustomProduct)

#### UDAS 

As seguintes UDAs precisam ser associadas a categoria do produto/sku a ser customizado

##### Engraving

|UDA|Valor|	 
|---|---|
| CUSTOM_PRODUCT |	110512,110513,110514,110515|
| CUSTOM_PRODUCT_CONFIG |{"customProductConfigs":[{"description":"customização de frase","positionName":"name","type":"name","customSkus":["110512","110513","110514","110515"],"required":true}]}|

##### Embossing

|UDA|Valor|	 
|---|---|
| CUSTOM_PRODUCT |	110512,110513,110514,110516 |
| CUSTOM_PRODUCT_CONFIG |{"customProductConfigs":[{"description":"customização de frase","positionName":"name","type":"name","customSkus":["110512","110513","110514","110516"],"required":true}]}|




##### Artigos

|Art ID | Finalidade |
|--- |--- |
|article-product-modal-embossing| Gravação |
|article-product-modal-engraving| Bordado |
|article-product-modal-refill| Refill |

#### Templates

Os templates cadastrados nos arigos precisam estar envoltos da seguinte tag

```
<script id="product-modal-engraving" type="x-tmpl-mustache">
	...
</script>
```

