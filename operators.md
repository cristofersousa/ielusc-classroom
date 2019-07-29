## Operadores

> Operadores aritméticos + , -, * , / e %

```
2+2
2-2
9/3 
4*4
```

> Operadores de atribuição += , -=, *=, /= e %= 

```
let result = 10;
result += 2;
result -= 5;
result *= 8;
result /= 2;
result %= 6;
```

> Operador de incremento ++ e decremento --

```
let result = 10;
result++;
++result;
result--;
--result;
```

> Operador binários |, &, ^, ~, <<, >> e >>>

```
4 | 3;
3 & 1;
5 ^ 2;
~2;
4 << 2;
128 >> 1;
-2 >>> 1;
```

Operadores binários são utilizados predominantente em algoritmos que interagem com este sistema de numeração, por exemplo: compressão, encriptação, comunicação de baixo nível para implementar validação de checksum e paridade, enfim, lugares onde as operações sejam feitas em números binários.

Em termos de performance se comparado a operadores normais, como existem muitos níveis de otimização acredito que não faça muita diferença. Muito adotado em eletrônica digital. Pode ser muito utilizado em frameworks IOT tal como Jhonny5 para trabalhar em conjunto com Arduíno.

Nota: Cuidado para não confundir os operadores | e & com || e &&