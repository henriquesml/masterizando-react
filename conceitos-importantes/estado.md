---
description: >-
  O Estado é onde você armazena valores das propriedades ou da lógica que
  pertencem ao componente.
---

# Estado

### Dê vida aos seus componentes

De nada vale uma interface bonita se ela é estática e está não faz nada. Um conceito muito importante dentro do React, são os estados, através dele damos ações, criamos condições e executamos algo dentro dos componentes.



### Exemplificando

A melhor maneira de entender claramente, é analisando um exemplo.

**O famoso contador:**

```jsx
import React, { useState } from 'react'

function Contador(){
  const [numero, setNumero] = useState(0)
    
  function adicionarNumero(){
    setNumero(numero + 1)
  }
    
  return(
    <div>
      <h1>{numero}</h1>
        <button onClick={() => adicionarNumero}
        >
          Adicionar
        </button>
    </div>
  )
}
```

### \#TODO

### Renderização

Quando um estado muda, o componente é renderizado novamente. Mas fique tranquilo, quem cuida disso é o React, nos só devemos orienta-lo a fazer isso corretamente.🧐 

