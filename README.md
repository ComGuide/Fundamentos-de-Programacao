# Fundamentos de programação

## Descrição

Este repositório contém um guia de estudos para a compreensão dos fundamentos de programação, com foco em na linguagem C.

---

## Tópicos

- [Instalando o compilador C/C++](https://github.com/ComGuide/Fundamentos-de-Programacao/tree/main/00_instalando)
- [Introdução à linguagem C](https://github.com/ComGuide/Fundamentos-de-Programacao/tree/main/01_introducao)
- [Variáveis e tipos de dados](https://github.com/ComGuide/Fundamentos-de-Programacao/tree/main/02_variaveis_e_tipos_de_dados)
- [Operadores aritméticos]
---

## ©️ Licença

Este repositório é licenciado sob a licença MIT. Você pode usar o conteúdo deste repositório para fins educacionais e não comerciais, desde que inclua a atribuição adequada. Consulte o arquivo LICENSE para obter mais informações.

---

## 📚 Referências
- [linguagemc](http://linguagemc.com.br/)
- [Instituto de Matemática e Estatística da Universidade de São Paulo - IME USP](https://www.ime.usp.br/~hitoshi/introducao/)
- [Documentação do Microsoft C++, C e Assembler](https://learn.microsoft.com/pt-br/cpp/c-language/?view=msvc-170)

# Documentação rápida

- [Compilando e executando um programa em C](#compilando-e-executando-um-programa-em-c)
- [Tipos de dados](#tipos-de-dados)
- [Imprimir dados](#imprimir-dados)
- [Ler dados](#ler-dados)

## Compilando e executando um programa em C

Comando para compilar um programa em C:

```shell
gcc nome_do_programa.c -o nome_do_programa_compilado
```

Comando para executar um programa em C:

Windows:
```shell
./nome_do_programa_compilado
```

Linux:
```shell
.\nome_do_programa_compilado
```

---

## Tipos de dados 

| Tipo de dado | Tamanho | Descrição | Exemplo | Intervalo | Formatação |
| :---: | :---: | :--- | :---: | :---: | :---: |
| `char` | 1 byte | Caractere | `'a'`, `'b'`, `'c'`, `'d'` | `0` a `255` | `%c` |
| `int` | 4 bytes | Inteiro | `0`, `1`, `2`, `3` | `-32768` a `32767`| `%d` |
| `float` | 4 bytes | Real | `0.0`, `1.0`, `2.0`, `3.0` | `-3.4E+38` a `3.4E+38` | `%f` |
| `double` | 8 bytes | Real | `0.0`, `1.0`, `2.0`, `3.0` | `-1.7E+308` a `1.7E+308` | `%lf` |
| `unsigned int` | 4 bytes | Inteiro sem sinal | `0`, `1`, `2`, `3` | `0` a `65535` | `%u` |
| `unsigned char` | 1 byte | Caractere sem sinal | `'a'`, `'b'`, `'c'`, `'d'` | `0` a `255` | `%c` |
| `long int` | 4 bytes | Inteiro longo | | `-2147483648` a `2147483647` | `%ld` |
| `unsigned long int` | 4 bytes | Inteiro longo sem sinal |  | `0` a `4294967295` | `%lu` |
| `long long int` | 8 bytes | Inteiro longo longo | | `-9223372036854775808` a `9223372036854775807` | `%lld` |
| `unsigned long long int` | 8 bytes | Inteiro longo longo sem sinal | | `0` a `18446744073709551615` | `%llu` |

---

## Imprimir dados
    
- Imprimindo um texto
    ```c
    printf("Hello World!");
    ```

- Imprimindo variáveis
    ```c
    int numero = 10;
    printf("%d", numero);
    ```

- Imprimindo variáveis com texto
    ```c
    int numero = 10;
    printf("O valor da variável numero é: %d", numero);
    ```

- Imprimindo variáveis com texto e quebra de linha
    ```c
    int numero = 10;
    printf("O valor da variável numero é: %d\n", numero);
    ```
---

## Ler dados

- Lendo um inteiro
    ```c
    int numero;
    scanf("%d", &numero);
    ```
- Lendo um caractere
    ```c
    char caractere;
    scanf("%c", &caractere);
    ```
- Lendo um real
    ```c
    float numero;
    scanf("%f", &numero);
    ```

---

## Operadores aritméticos


