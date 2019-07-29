## Variáveis

É possível declarar variáveis de diferentes formas, utilizando: 
`var, let e const`

## Ciclo de vida de uma variável

1. Declaração
2. Inicialização
3. Atribuição

- Declaração: O nome da variável é registrado no contexto de execução, também conhecido
como escopo, da função: 

- Inicialização: A variável é inicializada com o valor undefined

- Atribuição: Um valor é atribuído para a variável.

```
var name = 'JavaScript';
let dog = 'JavaScript';
const book  = 'JavaScript';
```

> Adotando var

Ao utilizar var, a variável é declarada e inicializada no escopo da função, não
respeitando bloco e permitindo a redeclaração e reatribuição. 

```
console.log(pi);

// undefined

var pi = 3.1415;
console.log(pi);

pi = 2;
constole.log(pi);

```

> Adotando let

Ao utilizar let, a variável é declarada no escopo da função mas só é inicializada
posteriormente, respeitando bloco e permitindo reatribuição mas não a redeclaração.

```
let pi =  3.1415;
console.log(pi);
pi = 3;
console.log(pi);
```

> Adotando const

Ao utilizar const, a variável é declarada no escopo da função mas só é inicializada
posteriormente, respeitando bloco e não permitindo reatribuição nem redeclaração.

```
const pi =  3.1415;
console.log(pi);
pi = 3;
console.log(pi);
```

Ao declarar uma variável sem `var, let ou const` ela é criada no escopo global.
**Nota**: Nunca declare variáveis sem var, let e const e evite a utilização de var.
  

  ## Identificadores válidos para variáveis

  Um identificar válido deve começar com [a-zA-Z_$] seguido por [a-zA-Z0-9_$]

  [+infos](https://stackoverflow.com/questions/4862193/difference-between-variable-declaration-syntaxes-in-javascript-including-global/4862268#4862268)