# Introdução a linguagem C

## Neste tópico você vai aprender

- [O que são bibliotecas](#📚o-que-são-bibliotecas)
- [Como criar um programa em C](#📝como-criar-um-programa-em-c)
- [Como compilar um programa em C](#🔧como-compilar-um-programa-em-c)
- [Como executar um programa em C](#🚀como-executar-um-programa-em-c)
- [Conclusão](#🎓conclusão)

---

## 📚O que são bibliotecas

Imagine que você precisa fazer um bolo. Para preparar um bolo é necessário ingredientes e utensílios de cozinha. Apesar de você saber como preparar um bolo, você não precisa saber como fazer um forno, uma batedeira ou uma forma de bolo. Você só precisa saber como usar esses utensílios para preparar o bolo.

Em programação, uma biblioteca é um conjunto de funções que você pode usar para fazer alguma coisa mesmo sem saber como essas funções foram implementadas. Por exemplo, nessa primeira etapa, aprenderemos a usar a função `printf` da biblioteca `stdio.h` para imprimir uma mensagem na tela. Mas não precisamos saber como essa função foi implementada, só precisamos saber como usá-la.

---

## 📝Como criar um programa em C

Para criar um programa em C, você precisa de um editor de texto. Você pode usar o bloco de notas, o notepad++, o vscode ou qualquer outro editor de texto. Neste primeiro momento, vamos usar o bloco de notas para criar um programa em C.

1. Abra o bloco de notas e digite o seguinte código:

    ```c
    1 #include <stdio.h>
    2
    3 int main() {
    4     printf("Hello World!");
    5     return 0;
    6 }
    ```

    O código acima é um programa em C que imprime a mensagem `Hello World!` na tela.

    É importante lembrar que para o código funcionar, você precisa digitar o código `exatamente` como está acima. Qualquer erro de digitação pode fazer com que o programa não funcione.

2. Salve o arquivo com o nome `hello.c` na área de trabalho ou em qualquer outro lugar que você preferir. É importante que o nome do arquivo termine com a extensão `.c`, pois essa extensão indica que o arquivo contém um programa em C.

    Antes de compilar o programa, vamos analisar o que cada linha desse código significa?

    - Na linha 1 do código, estamos dizendo ao compilador que precisamos da biblioteca `stdio.h.` Essa biblioteca contém a função `printf`, que é usada para imprimir mensagens na tela do computador. No caso deste código, estamos usando a função `printf` para imprimir a mensagem `"Hello World!"` na tela. Resumindo, a linha 1 é importante porque nos permite usar a função `printf` e exibir mensagens na tela do computador.

    - Na linha 3 do código, estamos declarando a função `main`. A função `main` é a função principal do programa. É a partir dela que o programa começa a ser executado.

    - Na linha 4 do código, estamos chamando a função `printf` para imprimir a mensagem `"Hello World!"` na tela.

    - Na linha 5 do código, estamos retornando o valor `0` para a função `main`. O valor `0` significa que o programa foi executado com sucesso. O código `return 0` é opcional, mas é uma boa prática de programação usá-lo.

---

## 🔧Como compilar um programa em C

Para compilar o programa que acabamos de criar, basta você seguir os passos abaixo:

1. Abra o prompt de comando e navegue até a pasta onde você salvou o arquivo `hello.c`. Para navegar até a pasta, você pode usar o comando `cd` (change directory). Por exemplo, se você salvou o arquivo `hello.c` na área de trabalho, você pode navegar até a pasta usando o comando `cd Desktop`. Caso você tenha entrado na pasta errada, você pode voltar para a pasta anterior usando o comando `cd ..`

2. Para compilar o programa, digite o seguinte comando no prompt de comando:

    ```bash
    gcc hello.c -o hello
    ```

    O comando acima compila o programa `hello.c` e gera um arquivo executável chamado `hello.exe`. O arquivo executável é o arquivo que contém o programa compilado. O comando `-o hello` indica que o arquivo executável deve ser chamado de `hello.exe`.

    Se o programa foi compilado com sucesso, você deve ver o arquivo `hello.exe` na pasta onde você salvou o arquivo `hello.c`.

---

## 🚀Como executar um programa em C

Para executar o programa que acabamos de compilar, basta você seguir os passos abaixo:

1. Ainda no prompt de comando e na pasta onde você compilou o programa, digite o seguinte comando:

    ```bash
    ./hello
    ```

    O comando acima executa o programa `hello.exe` e imprime a mensagem `Hello World!` na tela.

    a saída do programa deve ser parecida com a imagem abaixo:

    ```bash	
    PS C:\Users\joaon\Área de Trabalho> gcc hello.c -o hello
    PS C:\Users\joaon\Área de Trabalho> ./hello 
    Hello World!
    ```

---

## 🎓Conclusão

Agora que você já sabe como criar, compilar e executar um programa em C, você pode continuar aprendendo sobre a linguagem C. No próximo tópico, você vai aprender como declarar variáveis em C.

O código completo deste tópico está disponível [aqui](hello.c)

