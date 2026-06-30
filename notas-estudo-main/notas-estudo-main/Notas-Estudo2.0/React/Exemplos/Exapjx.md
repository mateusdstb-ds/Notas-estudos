## Exemplo App.jsx

```js

import { Route,Routes } from 'react-router-dom'

//import dos components 
import Header from './Components/Header'
import Footer from './Components/Footer'

//import das Pages 
import Home from './Pages/Home'
import Exercicio2 from './Pages/Exercicio2'
import Exercicio15 from './Pages/Exercicio15'

import './App.css'

function App() {
  return (
    <>
<Header /> 

<Routes>
<Route path='/Home' element={<Home />} /> 
<Route path='/Exercicio2' element={<Exercicio2 />} /> 
<Route path='/Exercicio15' element={<Exercicio15 />} /> 
</Routes>


<Footer />
    </>
  )
}

export default App

```