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


# Principais maneiras de testar localizadores DOCUMENT

Query Seletor:
```
document.querySelectorAll(‘cssSelector’);
```
Com uso de classe:

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/54658c6b-cad8-444b-901e-b141ff7d5c4a)

Com uso de ID:

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/ad34254e-c1c6-424d-bd29-61a49b4f94fb)


Get element:
```
document.getElementsByClassName(‘nomeClasse’);
```

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/aceefa85-907d-45a6-8f3e-b50cd80baaa3)

### _Xpaths_

```
document.evaluate('XPATH HERE', document, null, XPathResult.FIRST_ORDERED_NODE_TYPE, null).singleNodeValue;
```
![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/4440e6b4-8e89-414d-b268-ac4cab126979)

# Principais maneiras de testar localizadores CTRL + F

Testando seletor CSS:

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/fdf93049-52ae-40ab-b652-15c900b6090b)

Testando ID:

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/80cbe9a1-b699-401c-a504-40e856f4460c)



### Comandos mais utilizados:
### Seleção de todos os conteúdos, todos os elementos:

Comando:

```
$('*')
```

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/28355f22-4749-47c3-8093-20e0d1ba8068)


Caso queira fazer o mesmo com Xpath:
Comando:
```
//*
```
![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/67acffc4-7169-4bf3-a15c-c4f941007042)

Selecionando um elemento:
```
Comando: $(‘a’)
```
Nesse exemplo buscamos todos os elemento’a’.

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/e6db7690-8b8b-4c32-be44-21489620e3e1)


