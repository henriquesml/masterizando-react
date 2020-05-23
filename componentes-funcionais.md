# Componentes Funcionais

### Componentes como funções puras

Funções puras são chamadas assim porque elas nunca irão alterar suas entradas e sempre retornam o mesmo resultado para as mesmas entradas.

```jsx
function somar(a, b) {
  return a + b;
}
```

Em contraste, essa função é impura porque altera sua própria entrada:

```jsx
function withdraw(account, amount) {
  account.total -= amount;
}
```

React é bastante flexível mas tem uma única regra estrita:

**Todos os componentes React tem que agir como funções puras em relação ao seus props.**

