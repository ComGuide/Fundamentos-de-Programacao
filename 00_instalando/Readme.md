# Instalando o compilador C

## Neste tópico você vai aprender

- [O que é um compilador](#🖥️o-que-é-um-compilador)
- [O que é um arquivo binário](#🗃️o-que-é-um-arquivo-binário)
- [Como instalar o compilador C](#🔧como-instalar-o-compilador-c)
    - [Linux](#🐧no-linux)
    - [Windows](#💻no-windows)
- [Conclusão](#🎓conclusão)

---

## 🖥️O que é um compilador

Um compilador é um programa que transforma o código fonte em um arquivo executável. Ou seja, a partir de um arquivo de texto com instruções escritas em uma linguagem de programação, o compilador gera um arquivo binário que contém instruções que o processador do computador entende.

---

## 🗃️O que é um arquivo binário?

Um computador entende apenas instruções binárias, ou seja, instruções que são representadas por 0 e 1. Um arquivo binário é um arquivo que contém instruções binárias.

---

## 🔧Como instalar o compilador C

---

## 🐧No Linux

Para instalar o compilador C no Linux, abra o terminal e siga os passos abaixo:

1. Atualize o sistema

    ```bash
    sudo apt update
    ```
2. Instale o compilador C

    ```bash
    sudo apt install build-essential
    ```
3. Para testar, digite o seguinte comando no terminal:

    ```bash
    gcc --version
    ```


    Se tudo estiver correto, você verá uma mensagem parecida com esta:

    ```bash
    gcc (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
    Copyright (C) 2019 Free Software Foundation, Inc.
    This is free software; see the source for copying conditions.  There is NO
    warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
    ```

---

## 💻No Windows

Para instalar o compilador C no Windows, siga os passos abaixo:

1. Baixe o compilador C/C++ nessa pasta drive do Google: [MinGW](https://drive.google.com/drive/folders/16AHhoSSVjwti3Eg4TPve2UIxZSthp8Vx?usp=sharing)

2. Extraia o arquivo baixado para a pasta `C:\Program Files`

3. Adicione o caminho do compilador ao PATH do Windows. Para isso, siga os passos abaixo:

    1. Abra o menu iniciar e digite `variáveis de ambiente` e clique em `Editar as variáveis de ambiente do sistema`

    2. Clique em `Variáveis de ambiente`

    3. Na seção `Variáveis do sistema`, clique duas vezes em `Path`

    4. Clique em `Novo` e digite o caminho do compilador. Se você extraiu o arquivo para a pasta `C:\Program Files\MinGW\bin`

    5. Clique em `OK` e depois em `OK` novamente

4. Para testar, abra o prompt de comando e digite o seguinte comando:

    ```bash
    gcc --version
    ```
    Se tudo estiver correto, você verá uma mensagem parecida com esta:

    ```bash
    gcc (MinGW.org GCC-6.3.0-1) 6.3.0
    Copyright (C) 2016 Free Software Foundation, Inc.
    This is free software; see the source for copying conditions.  
    There is NO warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
    ```
---

## 🎓Conclusão

Agora que você já sabe o que é um compilador e como instalar o compilador C!

No próximo tópico, vamos aprender a escrever o nosso primeiro programa em C.
