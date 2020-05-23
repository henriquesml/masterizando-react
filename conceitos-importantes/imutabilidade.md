---
description: 'Entendesse por imutável, algo que não está sujeito a mudanças ou alterações.'
---

# Imutabilidade

A imutabilidade é importantíssima dentro da biblioteca, cada alteração de estado de um componente deve respeitar os seus princípios. Não devemos alterar da maneira tradicional como era feito antigamente no javascript.

**Errado**

```jsx
const pessoas = ['João', 'Maria']

pessoas.push('Bruxa')

atualizarPessoas(pessoas)
```

**Correto**

```jsx
const pessoas = ['João', 'Maria']

atualizarPessoas([...pessoas, 'Bruxa'])
```



