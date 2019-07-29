## Tipo de Dados:

Os tipos de dados na linguagem JavaScript se dividem em primitivos e objetos.

## Tipos Primitivos

Os primitivos são imutáveis, ou seja, ao longo do tempo seu valor não é alterado:

```
typeof 10;
typeof 'JavaScript';
typeof true;
typeof Symbol('iterator');
typeof null;
typeof undefined;
(10).toFixed(2);
(‘JavaScript’).replace(‘a’, ‘4’);
(true).toString();
(Symbol(‘iterator’)).toString();
```

## Objetos

Os objetos são valores que representam uma referência em memória que
pode ser alterada.

```

typeof function sum(a, b) { 
  return a + b} 
}
typeof {name: ‘Linus Torvalds’};
typeof [1,2,3,4,5,6];
typeof /[a-zA-Z]+/
typeof (new Date());

```

**Nota:** Cuidado, não confunda os operadores typeof e instanceof.