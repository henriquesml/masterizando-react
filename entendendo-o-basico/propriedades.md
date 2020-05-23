---
description: Propriedades são argumentos passados para um componente via atributos HTML.
---

# Propriedades

### React Props

As Propriedades \(comumente chamada de props\), são como argumentos de uma função ou atributos de um elemento HTML.

Para enviar atributos para um componente, usamos a mesma sintaxe HTML.

```jsx
<Carro marca="Fiat" nome="Uno"/>
```

Para recebermos as propriedades e manipularmos dentro do nosso componente, usamos a mesma sintaxe de uma função JavaScript.

```jsx
function Carro(props){
    return(
        <h1>Carro: {props.nome}</h1>
        <h1>Marca: {props.marca}</h1>
    )
}
```

Dentro de "props" no nosso componente Carro, está contido todas as propriedades do nosso componente. Em vez de pegarmos todas, podemos desestruturar as props e coletar as especificas que precisamos.

```jsx
// Ex: 1
function Carro(props){
    const {nome, marca} = props
    
    return(
        <h1>Carro: {nome}</h1>
        <h1>Marca: {marca}</h1>
    )
}

// Ex: 2

function Carro({nome, marca}){
    return(
        <h1>Carro: {nome}</h1>
        <h1>Marca: {marca}</h1>
    )
}
```

###  <a id="props-are-read-only"></a>

### Props são Somente Leitura <a id="props-are-read-only"></a>

Independente se você declarar um componente de forma de classe ou funcional, ele **nunca** deve modificar as suas próprias props. 

\*\*\*\*

