---
description: Componentes são partes independentes que juntos constituem a interface.
---

# Componentes

### Componentes são como funções

> "Conceitualmente, componentes são como funções JavaScript. Eles aceitam entradas arbitrárias \(chamadas “props”\) e retornam elementos React que descrevem o que deve aparecer na tela."



Separar sua aplicação em pequenos componentes é uma ótima pratica, ajuda a melhorar a manutenabilidade e o entendimento do código. Cada componente deve ser ser pensado de uma maneira que possibilite ser reutilizado e tratado isoladamente.



**Exemplo de Componente:**

```jsx
// Criação do Componente

function Ola(props) {
  return <h1>Olá, {props.nome}</h1>;
}
```

```jsx
// Chamada do componente

<Ola nome="Henrique Schmeller"/>

```



### Padrões de componentes

Muitos desenvolvedores abordam e tomam como prática o uso de **"um componente por arquivo"**, ou seja, cada arquivo estará destinado a somente um componente e neles estarão somente a lógica para a execução do seu proposito. Então juntamos todos e formamos a UI completa.🧩 



### Como saber quando uma parte da UI deve se tornar um componente?

Usando das mesmas técnicas que comumente são aplicadas para decidir se você deve ou não, criar uma nova função ou novo objeto. Uma dessas técnicas é o [princípio da responsabilidade única](https://en.wikipedia.org/wiki/Single_responsibility_principle), ou seja, um componente deve idealmente fazer apenas uma coisa. 

### 

### E se meu componente crescer?

Então ele deverá ser decomposto em subcomponentes menores.

### 

### Componentes devem ser feitos com classes ou funções?

As duas formas funcionam no React, porém a maneira indicada pelos desenvolvedores da biblioteca é através de funções. As atuais features do React \(hooks, por exemplo\) atendem melhor as funções e provem facilitadores que tornam o desenvolvimento **muito** melhor e mais fácil.





