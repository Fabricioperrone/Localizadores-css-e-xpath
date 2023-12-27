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
Retorna o valor do filtro de busca, 't-shirts'

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
document.querySelectorAll('cssSelector');
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
Comando: $('a')
```
Nesse exemplo buscamos todos os elemento’a’.

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/e6db7690-8b8b-4c32-be44-21489620e3e1)

Mesma consulta com Xpath:
```
Comando: $x('//a')
```

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/301add3e-6a90-429c-babe-7208ff553d01)

Consultando desde raiz com css: buscando elemento de uma determinada estrutura.

Comando: 
```
html > head > title
```

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/5a8cff13-eb43-4624-8e9f-97e45f289011)

Mesma consulta com Xpath:
```
/ html / head / title
```

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/baed9d2e-972d-4511-960a-99d19bb0bf7a)


Fazendo consultas usando filtro:

Vamos fazer uma consulta como se fosse um select em um banco de dados.

Comando:
```
$(‘input[name=”search_query”]’)
```

O que o comando faz: busca um _input_ na tela, onde o _name_ é igual a "search_query".

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/e35428b0-0d35-469b-86a8-ef108cc3e08c)


Agora vamos fazer o mesmo com _Xpath_:

Comando:
```
$x('//input[@name="search_query"]')
```
![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/11585fe1-a476-43d2-984d-4a7143a50c6a)


Comando: 
```
$('input[placeholder*="Sea"]')
```
![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/50e4ac96-ef88-40f1-bd73-41467e2fe51a)


Usando _*_ ele pesquisa todos os atributos que tenha "_placeholder_" e o valor desse atributo contenha o "_Sea_".

Vamos fazer a mesma consulta com _Xpath_:

Usando "_contains_":

Comando:
```
$x('//input[contains(@placeholder,"Sea")]')
```

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/9544075b-0ae5-4629-a72a-d787a2bb4e83)


### Quando não temos nenhum tipo de atributo:

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/ed2ce742-0554-4a0a-a93e-92294ed8d78d)

Comando:
```
$('form input:nth-child(4)')
```
Explicando o comando:

Nesse exemplo criamos um seletor sem usar id, class, name, placeholder. Somente utilizando elementos HTML.

![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/50bb4ef2-d403-4cf6-9ab5-f289e0f71e48)

Agora vamos fazer o mesmo com _Xpath_:

Comando: 
```
$x('//form//input[4]')
```
![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/1812573c-94a4-4a94-95cf-f344c4b128c0)


Pesquisando o primeiro elemento:

Comando:
```
$x('//form//input[1]')
``` 
![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/585b0099-a3bd-49f7-8c67-3a2c165bd165)

Buscando o _last_:

Comando:
```
$x('//form//input[last()]')
```
![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/16075779-b211-424a-886d-49828300256b)

Obs: nesse exemplo podemos ver que ele trouxe dois resultados, então não seria confiável, sempre busque por um elemento único.

Selecionando elemento pelo texto:

Comando: 
```
$x(‘//*[text()=”Lorem Ipsum”]’)
```
![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/5bf56079-950b-4585-b4d1-f8bce7d0ae76)

Usando "_contains_" junto com 	"_text_":

Comando: 
```
$x(‘//*[contains(text(), “textoexemplo”]’)
```
![image](https://github.com/Fabricioperrone/Localizadores-css-e-xpath/assets/69866913/0b13aad7-f682-4008-8056-7386ac21e537)


# Tabela de localizadores

| Nome                                 | CSS                                  | XPATH                                            |
|--------------------------------------|--------------------------------------|--------------------------------------------------|
| Todos os elementos                   | *                                    | //*                                              |
| Um elemento                          | p                                    | //p                                              |
| Caminho absoluto                     | html > body > title                  | /html/body/title                                 |
| Query com atributo                   | Input[placeholder=”Search”]          | //input[@placeholder, “Search”]                  |
| Query com parte de atributo          | Input[placeholder*=”Sea”]            | //input[contains(@placeholder, “Sear”)]           |
| Filhos do elemento                   | Form input:first-child               | //form/input[1]                                  |
|                                      | Form input:nth-child(4)              | //form/input[4]                                  |
|                                      | Form input:first-child               | //form/input[1]                                  |
| Classe e id                          | .sear_query                          | //*[@class=”search_query form-control ac_input”] |
|                                      | #search_query_top                    | //*[@id=”search_query_top”]                      |
|                                      |                                      | //*[contains(@class, “search_query”)]            |
| Elemento pelo seu texto              |                                      | //*[text()=”Come Visit Us”]                      |
|                                      |                                      | //*[contains(text(), “Nort Carolina”)]           |


Fonte: Iterasys Live com: [Danilo Arantes Freitas](https://www.youtube.com/watch?v=ZSAglCvKy9g&ab_channel=Iterasys)

### Agradecimentos:

> Gostaria de agradecer ao meu amigo Sandro Augusto por me ajudar nesse projeto  [Linkedin](linkedin.com/in/sandro-augusto-774a6a140)
