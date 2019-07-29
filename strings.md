## Strings

O tipo String é primitivo, imutável e é representado internamente pelo padrão
Unicode, codificado em UTF-16

Existem 3 formas de declarar uma String de forma literal: aspas simples, aspas
duplas ou acento grave.

```
'JavaScript"
'JavaScript'
`Javascript`
```

Se compararamos essas formas de Strings o que será que o JavaScript nos retorna?

'JavaScript' === "JavaScript"
// true

Também é possível declarar uma String por meio da sua função construtora.

```
new String('JavaScript');
new String(`JavaScript`);
new String("JavaScript");
```

Nota: A função construtora é mais lenta e pode prejudicar a performance.

```
let counter = 0;
console.time('performance');
while (counter < 100000) {
  'JavaScript'; 
   counter++ ;
}
console.timeEnd('performance');



let counter = 0;
console.time('performance');
while (counter < 100000) {
  'new String('JavaScript'); 
   counter++ ;
}
console.timeEnd('performance');
```

## Template Literal

Um template literal é uma forma de declarar uma String que permite a
interpolação de expressões.

````
let host = "localhost";
let port = "3000";
let resource = "users";
let url = "https://" + host + ":" + port + "/" + resource;
console.log(url);
```

```
let host = "localhost";
let port = "3000";
let resource = "users";
let url = `https://${host}:${port}/${resource}`;
console.log(url);
````

Além da interpolação de expressões é possível também declarar uma String
multi linha, sem a necessidade de caracteres especiais

``` 

let monthsOfYear = 
"0 - Jan" + 
"1 - Feb" + 
"2 - Mar" + 
"3 - Apr" + 
"4 - May" + 
"5 - Jun" +
"6 - Jul" +
"7 - Aug" +
"8 - Sep" +
"9 - Oct" + 
"10 - Nov" +
"11 - Dec"
console.log(monthsOfYear);

```


## String API

- length: Retorna o tamanho da String
- indexOf: Retorna a primeira posição encontrada do
caractere passado por parâmetro
- lastIndexOf: Retorna a última posição encontrada
do caractere passado por parâmetro
- toUpperCase: Retorna uma nova String
convertendo as letras para maiúsculas
- toLowerCase: Retorna uma nova String
convertendo as letras para minúsculas

```
'JavaScript'.length;
'PHP'.indexOf('P');
'PHP'.lastIndexOf('P');
'cobol'.toUpperCase();
'ALGOL'.toLowerCase();
```


- charAt: Retorna o caractere na posição passada por parâmetro
- charCodeAt: Retorna o código com base na posição passada por parâmetro
- fromCharCode: Retorna um caractere com base no código passado por parâmetro

```
'JavaScript'.charAt(1);
'JavaScript'.charCodeAt(1);
String.fromCharCode(97);
```

- includes: Retorna verdadeiro se a String contém a String passada por parâmetro
- startsWith: Retorna verdadeiro se a String inicia com a String passada por parâmetro
- endsWith: Retorna verdadeiro se a String termina com a String passada por parâmetro

```
'JavaScript'.includes('Java');
'Ruby'.startsWith('R');
'Erlang'.endsWith('lang');
```


- localeCompare: Retorna -1 se a String passada por parâmetro for maior, 0 se for igual e 1 se for menor

```
'C++'.localeCompare('Ruby');
'Python'.localeCompare('Java');
'JavaScript'.localeCompare('JavaScript');

```

- match: Retorna partes da String com base na RegExp passada por parâmetro
- search: Retorna a primeira posição encontrada com base na RegExp passada por parâmetro
- replace: Retorna uma nova String resultante da substituição da String ou RegExp passada no primeiro parâmetro pelo segundo parâmetro

```
'C++'.match(/\+/g);
'Java'.search(/a/);
'JavaScript'.replace('Java', 'Ecma');
'JavaScript'.replace(/a/g, 4);
```



- slice: Retorna uma parte da String que está invocando a função iniciando na posição passada no primeiro parâmetro até a posição final passada no segundo parâmetro, ou da posição passada no primeiro parâmetro até o fim caso o segundo parâmetro não seja informado
- split: Retorna um array contendo o resultado da divisão da String original de acordo com o critério passado por parâmetro
- substring: Similar ao slice, não aceita valores negativos como parâmetro e permite a inversão dos parâmetros

```
'JavaScript'.slice(0, 4);
'JavaScript'.slice(4);
'JavaScript'.slice(0, -6);
'JavaScript'.slice(-6);
'C;Java;JavaScript;Ruby'.split(';');
'JavaScript'.substring(0, 4);
'JavaScript'.substring(4, 0);
'JavaScript'.substring(4);


```


- concat: Retorna uma nova String resultante da concatenação da que está invocando a função e da outra, passada por parâmetro
- padStart: Completa a String com caracteres no início
- padEnd: Completa a String com caracteres no fim
- repeat: Repete um caractere
- trim: Elimina espaços em branco no início e no fim
- trimLeft: Elimina espaços em branco no início
- trimRight: Elimina espaços em branco no fim

```
'Java'.concat('Script');
'Data'.concat('Flex');
'Script'.padStart(10, 'Java');
'C'.padEnd(3, '+');
'C'.concat('+'.repeat(2));
' Self '.trim();
' Scheme '.trimLeft();
' Perl '.trimRight();
```