# Localizadores CSS & Xpath

o que você vai aprender?

- Saber diferenciar entre expressões CSS e Xpath;
- Conhecer maneiras para testar localizadores;
- Identificar elementos HTML, atributos e seus valores;
- Conseguir montar seu seletor CSS e Xpath;
- Quando usar cada um.

## DOCUMENT OBJECT MODEL

![DOM](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/95108ce2-2ef7-47cd-b720-68d88b0a618b)


## Ainda sobre HTML:
![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/98077169-7194-4ad9-abf1-a4c754f7d290)


-	Qual é o tipo do elemento? O elemento é o que vem depois do sinal de maior >, nesse exemplo seria o “select”.
-	Quais são seus atributos? São todos os itens que estão antes do sinal de “=”.
-	Quais são os valores de seus atributos? Nesse exemplo são: países, left-align, Seleção de países.


### Guardem esses conceitos:

>  Qual é o tipo do elemento?
> 
>  Quais são seu atributos?
> 
>  Quais são os # valores de seus atributos?

### Tipos de localizadores
- Xpath
- Atribute
- Name
- ID
- CSS Selector
- Class name
- Link text
- Tag name

### Um pouco de cada um
## Xpath:
- XML Path Language (Linguagem de XML);
- Se parecem com caminhos de diretórios.
  
Exemplo:
  - /html/head/title
### CSS Seletor
- Seletores CSS são expressões para locaiizar um elemento;

Exemplo:
  - div p


## Principais maneiras de testar localizadores _JQuery_

Sintaxe _JQuery_

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/08731438-ba4d-4217-a193-63294020d2b5)


Site com localizadores _CSS_ & _Xpath_ [Cheatsheet](https://devhints.io/xpath)
 
### Hand´s on!
```
CSS: $('.search_query').val()
``` 
Retorna o valor do filtro de busca, ‘t-shirts’

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/60338f49-1c15-4ae4-a77f-d54dfe3a62d8)

```
$('.homefeatured').text()
```
Retorna o texto

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/d117d296-adc9-4d67-8624-5df9f86e5770)

```
$('.blockbestsellers:first-child')
```
Retorna somente a primeira ocorrência daquele seletor _CSS_.

```
$('.blockbestsellers:first-child').click
```
Testa se o seletor funciona com .click()

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/ee2d67c5-a377-4b0b-ace1-d3fc0a7296b6)


```
$('.search_query').val('T-SHIRTS')
```

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/52b702e9-0fdf-4f43-a03a-a0f23e57a236)

Exemplo com _Xpath_:

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/d2757c63-90bb-4b9b-86fa-cdccdb84700c)

//div

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/3f74fc64-1b05-49e3-94a7-a5dbf14e4940)




