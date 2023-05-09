# Operadores aritméticos

## Neste tópico você aprenderá sobre:

- [Para que servem os operadores aritméticos](#🧮para-que-servem-os-operadores-aritméticos)
- [Operadores aritméticos](#🧮operadores-aritméticos)
- [Ordem de precedência dos operadores aritméticos](#🧮ordem-de-precedência-dos-operadores-aritméticos)
- [Operadores de incremento e decremento](#🧮operadores-de-incremento-e-decremento)
- [Operações entre tipos de dados diferentes](#🧮operações-entre-tipos-de-dados-diferentes)
- [Conclusão](#🎓conclusão)

---


## 🧮Para que servem os operadores aritméticos

Os operadores aritméticos são utilizados para realizar operações matemáticas entre variáveis e constantes. Vale lembrar que uma constante não pode ser alterada durante a execução do programa, mas ela pode ser utilizada para realizar operações mateḿaticas.

---

## 🧮Operadores aritméticos

| Operador | Descrição | Exemplo | Resultado |
| :---: | :--- | :---: | :---: |
| + | Adição | 2 + 2 | 4 |
| - | Subtração | 2 - 2 | 0 |
| * | Multiplicação | 2 * 2 | 4 |
| / | Divisão | 2 / 2 | 1 |
| % | Módulo | 2 % 2 | 0 |

Com exceção do operador módulo, todos os outros operadores aritméticos funcionam da mesma forma que na matemática. O operador módulo retorna o resto da divisão entre dois números inteiros.

### Vamos ver alguns exemplos de operações aritméticas:

Operação de adição:

```c
#include <stdio.h>

int main() {

    int valor_1 = 10;
    int valor_2 = 5;

    int soma = valor_1 + valor_2;

    printf("A soma de %d e %d é %d\n", valor_1, valor_2, soma);

    return 0;
}
```
Saída do programa:

```shell
A soma de 10 e 5 é 15
```

Operação de subtração:

```c
#include <stdio.h>

int main() {

    int valor_1 = 10;
    int valor_2 = 5;

    int subtracao = valor_1 - valor_2;

    printf("A subtração de %d e %d é %d\n", valor_1, valor_2, subtracao);

    return 0;
}
```
Saída do programa:

```shell
A subtração de 10 e 5 é 5
```

Operação de multiplicação:

```c
#include <stdio.h>

int main() {

    int valor_1 = 10;
    int valor_2 = 5;

    int multiplicacao = valor_1 * valor_2;

    printf("A multiplicação de %d e %d é %d\n", valor_1, valor_2, multiplicacao);

    return 0;
}
```

Saída do programa:

```shell
A multiplicação de 10 e 5 é 50
```

Operação de divisão:

```c
#include <stdio.h>

int main() {

    int valor_1 = 10;
    int valor_2 = 5;

    int divisao = valor_1 / valor_2;

    printf("A divisão de %d e %d é %d\n", valor_1, valor_2, divisao);

    return 0;
}
```

Saída do programa:

```shell
A divisão de 10 e 5 é 2
```

Operação de módulo:

```c
#include <stdio.h>

int main() {

    int valor_1 = 10;
    int valor_2 = 5;

    int modulo = valor_1 % valor_2;

    printf("O módulo de %d e %d é %d\n", valor_1, valor_2, modulo);

    return 0;
}
```

Saída do programa:

```shell
O módulo de 10 e 5 é 0
```

---

## 🧮Ordem de precedência dos operadores aritméticos

A ordem de precedência dos operadores aritméticos é a mesma da matemática. A ordem de precedência é a seguinte:

1. Parênteses
2. Multiplicação, divisão e módulo
3. Adição e subtração

### Vamos ver alguns exemplos de operações aritméticas com ordem de precedência:

```c
#include <stdio.h>

int main() {

    int valor_1 = 10;
    int valor_2 = 5;
    int valor_3 = 2;

    int resultado = valor_1 + valor_2 * valor_3;

    printf("O resultado da operação é %d\n", resultado);

    return 0;
}
```

Saída do programa:

```shell
O resultado da operação é 20
```
Veja que o resultado da operação foi 20, pois a multiplicação foi realizada antes da adição. Se quisermos que a adição seja realizada antes da multiplicação, devemos utilizar parênteses:

```c
#include <stdio.h>

int main() {

    int valor_1 = 10;
    int valor_2 = 5;
    int valor_3 = 2;

    int resultado = (valor_1 + valor_2) * valor_3;

    printf("O resultado da operação é %d\n", resultado);

    return 0;
}
```

Saída do programa:

```shell
O resultado da operação é 30
```

---

## 🧮Operadores de incremento e decremento

Os operadores de incremento e decremento são utilizados para incrementar ou decrementar o valor de uma variável. Os operadores de incremento e decremento são representados pelos símbolos ++ e --, respectivamente.

### Vamos ver alguns exemplos de operadores de incremento e decremento:

### Incremento:

```c
#include <stdio.h>

int main() {

    int valor = 10;

    valor++;

    printf("O valor é %d\n", valor);

    return 0;
}
```

Saída do programa:

```shell
O valor é 11
```

### Decremento:

```c
#include <stdio.h>

int main() {

    int valor = 10;

    valor--;

    printf("O valor é %d\n", valor);

    return 0;
}
```

Saída do programa:

```shell
O valor é 9
```

### Incremento e decremento antes e depois da variável:

Os operadores de incremento e decremento podem ser utilizados antes ou depois da variável. Quando o operador é utilizado antes da variável, o valor da variável é incrementado ou decrementado antes de ser utilizado. Quando o operador é utilizado depois da variável, o valor da variável é incrementado ou decrementado depois de ser utilizado.

### Vamos ver alguns exemplos de operadores de incremento e decremento antes e depois da variável:

### Incremento antes da variável:

```c
#include <stdio.h>

int main() {

    int valor = 10;

    ++valor;

    printf("O valor é %d\n", valor);

    return 0;
}
```

Saída do programa:

```shell
O valor é 11
```

### Decremento antes da variável:

```c
#include <stdio.h>

int main() {

    int valor = 10;

    --valor;

    printf("O valor é %d\n", valor);

    return 0;
}
```

Saída do programa:

```shell
O valor é 9
```

# 🧮Operações entre tipos de dados diferentes

## 🧮Operações entre inteiros e ponto flutuante

Quando realizamos operações entre inteiros e ponto flutuante, o resultado da operação é um ponto flutuante.

### Vamos ver alguns exemplos de operações entre inteiros e ponto flutuante:

```c
#include <stdio.h>

int main() {

    int valor_1 = 10;
    float valor_2 = 5.5;

    float soma = valor_1 + valor_2;

    printf("A soma de %d e %f é %f\n", valor_1, valor_2, soma);

    return 0;
}
```

Saída do programa:

```shell
A soma de 10 e 5.500000 é 15.500000
```

Atenção: Quando realizamos operações entre diferentes tipos, podemos ter perda de informação. Por exemplo, se realizarmos uma operação entre um inteiro e um ponto flutuante, o resultado da operação será um ponto flutuante, mas o valor será truncado, ou seja, o valor será arredondado para baixo.

### Vamos ver um exemplo de perda de informação:

```c
#include <stdio.h>

int main() {

    int valor_int = 10;
    float valor_float = 5.5;

    int soma = valor_int + valor_float;

    printf("A soma de %d e %f é %d\n", valor_int, valor_float, soma);

    return 0;
}
```

Saída do programa:

```shell
A soma de 10 e 5.500000 é 15
```

Veja que o resultado da operação foi 15, pois o valor 5.5 foi truncado para 5.

## 🧮Operações entre inteiros e caracteres

Quando realizamos operações entre inteiros e caracteres, o resultado da operação é um inteiro, pois os caracteres são representados por números na tabela [ASCII](https://www.ime.usp.br/~pf/algoritmos/apend/ascii.html).

### Vamos ver alguns exemplos de operações entre inteiros e caracteres:

```c
#include <stdio.h>

int main() {

    int valor_int = 10;
    char valor_char = 'a';

    int soma = valor_int + valor_char;

    printf("A soma de %d e %c e %d\n", valor_int, valor_char, soma);

    return 0;
}
```

Saída do programa:

```shell
A soma de 10 e a e 107
```

Veja que o resultado da operação foi 107, pois o caractere 'a' é representado pelo número 97 na tabela ASCII.

---

# 🎓Conclusão

Após este tópicos, você já sabe como realizar operações aritméticas em C. Agora, você já pode resolver os exercícios com operações aritméticas.