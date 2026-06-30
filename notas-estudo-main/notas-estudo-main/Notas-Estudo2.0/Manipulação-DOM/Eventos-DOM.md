## Eventos 

# Click

```js 

Disparado quando um elemento é clicado 

Exemplo: const button= document.getElementById("My-button")
button.addEventListener("click" , ()=>{
    alert("Button was clicked")
    })
```
# Submit 

```js 
Disparado quando um formulário é enviado 

document.querySelector("form").addEventListener("submit", (event) => {
    event.preventDefault(); //previne que a pagina recarregue 
    console.log("Form submitted");
})

```

# mouseover

```js
Disparado quando o ponteiro do mouse passsa sobre um elemento .

document.querySelector("div").addEventListener("mouseover",() => {
    console.log("Mouse over the div")
})

```

# keydown

```js 
Dispara quando uma tecla é precionada .

documents.addEventListener("keydown",(event)  => {
    console.log("key pressed : ${event.key}");
})

```

# Função 

```js

Ela so executara o codigo que estara dentro dela quando for chamada .

Exemplo :

function exemplo(){

}

const buttonExercicio3 = document.getElementById("exercicio3")
buttonExercicio3.addEventListener("click", () => { exemplo() })

```