# Variáveis e tipos de dados

## Neste tópico, você vai aprender:

- [O que é uma variável](#📦o-que-é-uma-variável)
- [O que é um tipo de dado](#📝o-que-é-um-tipo-de-dado)
- [Como declarar uma variável](#📦como-declarar-uma-variável)
- [Como atribuir um valor a uma variável](#📦como-atribuir-um-valor-a-uma-variável)
- [Como imprimir o valor de uma variável](#📦como-imprimir-o-valor-de-uma-variável)
- [Como ler o valor de uma variável](#📦como-ler-o-valor-de-uma-variável)
- [Modificando o valor de uma variável](#📦modificando-o-valor-de-uma-variável)
- [Como declarar uma constante](#📦como-declarar-uma-constante)
- [Conclusão](#🎓conclusão)

---

## 📦O que é uma variável?

Uma variável é um espaço na memória do computador que armazena um valor. Como o nome sugere, o valor armazenado pode variar, ou seja, pode ser alterado durante a execução do programa para representar diferentes valores e realizar diferentes tarefas.

---

## 📝O que é um tipo de dado?

Um tipo de dado é uma classificação que define quais valores podem ser armazenados em uma variável. Por exemplo, uma variável do tipo `int` pode armazenar apenas números inteiros, enquanto uma variável do tipo `float` pode armazenar números reais.

Em C temos os seguintes tipos de dados:

| Tipo de dado | Tamanho | Descrição | Exemplo | Intervalo |
| :---: | :---: | :--- | :---: | :---: |
| `char` | 1 byte | Caractere | `'a'`, `'b'`, `'c'`, `'d'` | `0` a `255` |
| `int` | 4 bytes | Inteiro | `0`, `1`, `2`, `3` | `-32768` a `32767`|
| `float` | 4 bytes | Real | `0.0`, `1.0`, `2.0`, `3.0` | `-3.4E+38` a `3.4E+38` |
| `double` | 8 bytes | Real | `0.0`, `1.0`, `2.0`, `3.0` | `-1.7E+308` a `1.7E+308` |
| `void` | 0 byte | Vazio | - | - |

Também podemos ter algumas variações desses tipos de dados, como `unsigned int`, `long int`, `long long int`, `long double`, etc.

| Variação | Descrição | Exemplo | 
| :---: | :--- | :---: |
| `unsigned int` | Inteiro sem sinal | `0`, `1`, `2`, `3` |
| `unsigned char` | Caractere sem sinal | `'a'`, `'b'`, `'c'`, `'d'` |
| `long int` | Inteiro longo | `-2147483648` a `2147483647` |
| `unsigned long int` | Inteiro longo sem sinal | `0` a `4294967295` |
| `long long int` | Inteiro longo longo | `-9223372036854775808` a `9223372036854775807` |
| `unsigned long long int` | Inteiro longo longo sem sinal | `0` a `18446744073709551615` |

Você pode ver que existe várias variações de tipos de dados, mas não se preocupe com isso agora. Vamos focar nos tipos de dados mais comuns, que são `char`, `int`, `float` e `double`.

---

## 📦Como declarar uma variável?

Para declarar uma variável, você deve informar o tipo de dado que ela vai armazenar e um nome para ela. Por exemplo, para declarar uma variável do tipo `int` com o nome `idade`, você deve escrever o seguinte código:

```c
#include <stdio.h>

int main() {
    int idade;
    return 0;
}
```

O código acima declara uma variável do tipo `int` com o nome `idade`. Note que o nome da variável deve seguir algumas regras:

- O nome deve começar com uma letra ou com o caractere `_`.
    - Exemplos: `idade`, `_idade`, `idade_`.
- O nome pode conter apenas letras, números e o caractere `_`.
    - Exemplos: `idade`, `idade_1`, `idade_2`, `idade_3`.
- O nome não pode conter espaços.
    - Exemplos: `idade 1`, `ida de`.
- O nome não pode ser uma palavra reservada da linguagem C.
    - Exemplos: `int`, `continue`, `break`.

---

## 📦Como atribuir um valor a uma variável?

Para atribuir um valor a uma variável, você deve usar o operador de atribuição `=`. Por exemplo, para atribuir o valor `10` à variável `idade`, você deve escrever o seguinte código:

```c
#include <stdio.h>

int main() {
    int idade;
    idade = 10;
    return 0;
}
```

O código acima atribui o valor `10` à variável `idade`. Note que o valor atribuído deve ser compatível com o tipo de dado da variável. Por exemplo, se a variável for do tipo `int`, o valor atribuído deve ser um número inteiro. Se a variável for do tipo `float`, o valor atribuído deve ser um número real.

Outros exemplos:

```c
#include <stdio.h>

int main() {
    float altura;
    altura = 1.75;
    return 0;
}
```

```c
#include <stdio.h>

int main() {
    char letra;
    letra = 'a';
    return 0;
}
```

---

## 📦Como imprimir o valor de uma variável?

Note que os código que escrevemos até agora não fazem nada. Para que o programa faça alguma coisa, precisamos imprimir o valor da variável para o usuário.

Para imprimir o valor de uma variável, você deve usar a função `printf()`. Por exemplo, para imprimir o valor da variável `idade`, você deve escrever o seguinte código:

```c
#include <stdio.h>

int main() {
    int idade;
    idade = 10;
    printf("%d", idade);
    return 0;
}
```

O código acima imprime o valor da variável `idade`.

A saída do programa após ser compilado e executado será:
    
```shell
10
```

Note que o formato de impressão `%d` deve ser compatível com o tipo de dado da variável. Por exemplo, se a variável for do tipo `int`, o formato de impressão deve ser `%d`. Se a variável for do tipo `float`, o formato de impressão deve ser `%f`.

Veja a tabela abaixo para saber quais formatos de impressão devem ser usados para cada tipo de dado:

| Tipo de dado | Formato de impressão |
| :---: | :---: |
| `char` | `%c` |
| `int` | `%d` |
| `float` | `%f` |
| `double` | `%lf` |
| `long int` | `%ld` |
| `long long int` | `%lld` |
| `unsigned int` | `%u` |
| `unsigned long int` | `%lu` |
| `unsigned long long int` | `%llu` |

Apesar de existir vários formatos de impressão, não se preocupe com isso agora. Vamos focar nos formatos de impressão mais comuns, que são `%c`, `%d`, `%f` e `%lf`.

Outros exemplos:

```c
#include <stdio.h>

int main() {
    float altura;
    altura = 1.75;
    printf("%f", altura);
    return 0;
}
```

```c
#include <stdio.h>

int main() {
    char letra;
    letra = 'a';
    printf("%c", letra);
    return 0;
}
```

```c
#include <stdio.h>

int main() {
    double preco;
    preco = 10.50;
    printf("%lf", preco);
    return 0;
}
```
Tente compilar e executar os códigos acima para ver o resultado.

---

## 📦Como ler o valor de uma variável?

Para ler o valor de uma variável, você deve usar a função `scanf()`. Ela é responsável por ler o valor digitado pelo usuário e armazenar na variável. Por exemplo, para ler o valor da variável `idade`, você deve escrever o seguinte código:

```c
#include <stdio.h>

int main() {
    int idade;

    printf("Digite sua idade: ");
    scanf("%d", &idade);

    printf("A sua idade e: %d", idade);

    return 0;
}
```

O código acima lê o valor da variável `idade` e imprime na tela.

A entrada e saída do programa após ser compilado e executado será:

```shell
Digite sua idade: 10
A sua idade e: 10
```

Note que dessa vez utilizamos o caractere `&` antes do nome da variável. Isso é necessário porque a função `scanf()` precisa saber o endereço de memória da variável para armazenar o valor digitado pelo usuário.

o caractere `&` é chamado de operador de endereço. Ele é usado para obter o endereço de memória de uma variável. Por exemplo, para obter o endereço de memória da variável `idade`, você deve escrever o seguinte código:

```c
#include <stdio.h>

int main() {
    int idade;

    printf("O endereco de memoria da variavel idade e: %p", &idade);

    return 0;
}
```

A saída do programa após ser compilado e executado será parecida com isso:

```shell
O endereco de memoria da variavel idade e: 0x7ffeedb0a4fc
```

Veja que apareceu vários números e letras sem sentido. Isso é o endereço de memória da variável `idade`. Cada variável tem um endereço de memória diferente.

---

## 📦Modificando o valor de uma variável

Para modificar o valor de uma variável, você deve usar o operador de atribuição `=`. Por exemplo, para modificar o valor da variável `idade`, você deve escrever o seguinte código:

```c
#include <stdio.h>

int main() {
    int idade;

    idade = 10
    printf("A sua idade e: %d", idade);

    idade = 20;
    printf("A sua nova idade e: %d", idade);

    return 0;
}
```

A saída do programa após ser compilado e executado será:

```shell
A sua idade e: 10
A sua nova idade e: 20
```

Note que o valor da variável `idade` foi modificado de `10` para `20`. pois atribuímos o valor `20` à variável `idade` durante a execução do programa.

---

## 📦Como declarar uma constante

Uma constante é um valor que não pode ser alterado durante a execução do programa. Para declarar uma constante, você deve usar a palavra-chave `const`. Por exemplo, para declarar uma constante chamada `PI`, você deve escrever o seguinte código:

```c
#include <stdio.h>

int main() {
    const float PI = 3.14;
    printf("O valor de PI e: %f", PI);
    return 0;
}
```

A saída do programa após ser compilado e executado será:

```shell
O valor de PI e: 3.140000
```

Note que o valor da constante `PI` não pode ser alterado durante a execução do programa. Se você tentar alterar o valor da constante `PI`, o compilador irá gerar um erro.

```c
#include <stdio.h>

int main() {
    const float PI = 3.14;
    PI = 3.1415;
    printf("O valor de PI e: %f", PI);
    return 0;
}
```

A saída do programa após ser compilado e executado será:

```shell
error: assignment of read-only variable 'PI'
```

---

## 🎓Conclusão

Agora você já sabe como declarar variáveis e constantes em C. Você também aprendeu como imprimir o valor de uma variável na tela e como ler o valor digitado pelo usuário.










