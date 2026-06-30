## DOM -> Document Object Model

```js 

Representação Estrutural : O DOM é uma representação estruturada do documento html em forma de árvore , onde cada tag HTML é representada como um nó . Isso permite que script , como JavaScript , interajam e manipulem o conteúdo da página .

A estrutura semântica e hierárquica do DOM facilita a navegação para tecnologias assistivas ,como leitores de tela .

```

## getElementById

```js 

função : Retorna uma referência ao elemento pelo seu ID . 

Uso principal : Selecionar elementos únicos em uma página para manipulação ou leitura  de dados

Exemplo :

const element=document.getElementById('my-element');
element.style.color = 'blue';

```
# querySelector 

```js 

Função : Retornar o primeiro elemento que corresponde ao seletor CSS especificado .

Uso principal : Selecionar qualquer elemento usando seletores CSS, permitindo mais flexibilidade que getElementById.

Exemplos :

```js 
const element= document.querySelector("my-class");

element.style.backgroundColor ="yellow"; 
```

# Create Element 

```js 

Função : cria novo elemento HTML .

Uso principal : Adicionar novos elementos  à páginas dinamicamente .

Exemplo :

const newDiv = document.createElement("div");
newDiv.textContent ="Hello,World !";
document.body.appendChild(newDiv);
```

# appendChild

```js 

Função Adiciona um nó (elemento) como o último filho de um elemento pai especificado 

Uso principal : Inserir elementos novos ou existentes na árvore DOM .

Exemplo :

const parent = document.getElementById("parent-element");
const child = document.createElement("p");
child.textContent = "This is a new paragraph";
parent.appendChild(child)
```
