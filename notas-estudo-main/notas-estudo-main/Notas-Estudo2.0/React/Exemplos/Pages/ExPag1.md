## Exemplo page 1

```js 

//import do css
import './style.css'

import { useState } from 'react'

//import das rotas 
import { Link } from 'react-router-dom'


function Exercicio2(){
    const[ numero1,setNumero1]=useState('')
     const[ numero2,setNumero2]=useState('')
    const [resultado,setResultado]=useState()

function conta(event){
    event.preventDefault()

setResultado(Number(numero1)*Number(numero2))

}

    return(
<>

<form onSubmit={conta}>
<label htmlFor="text">Qual a quantidade que você ganha por hora </label>
<input
 type="text"
 value={numero1}
 onChange={(event)=> setNumero1 (event.target.value)}
 />

<label htmlFor="text">Qual a quantidade de horas trabalhadas no mes</label>
<input
 type="text"
 value={numero2}
 onChange={(event)=> setNumero2 (event.target.value)}
 />


<button type='submit' onClick={conta}>resultado</button>
</form>

<p>{resultado}</p>
</>
    )
}

export default Exercicio2

```