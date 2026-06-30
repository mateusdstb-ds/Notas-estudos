## Exemplo home

```js
import './style.css'


//import das rotas 
import { Link } from 'react-router-dom'

function Home(){
    return(
        <>
        <Link to='/Exercicio2'><button>Exercicio 2 </button></Link>
            <Link to='/Exercicio15'><button>Exercicio 15 </button></Link>
        </>
    )
}
export default Home 
```