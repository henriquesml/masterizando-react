---
description: Uma função pura sempre trás os mesmos resultados para as mesmas entradas
---

# Componentes Funcionais

### Componentes puramente funcionais[ λ](https://pt.wikipedia.org/wiki/Programa%C3%A7%C3%A3o_funcional)

Funções puras são chamadas assim porque elas nunca irão alterar suas entradas e sempre retornarão o mesmo resultado para as mesmas entradas.

```jsx
function somar(a, b) {
  return a + b;
}
```



Em contraste, uma função impura é chamada assim porque altera sua própria entrada:

```jsx
function withdraw(account, amount) {
  account.total -= amount;
}
```



Esse conceito é muito importante para o principio de [Propriedades](../propriedades.md) que veremos à seguir.

