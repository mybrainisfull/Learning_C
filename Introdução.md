# Função main()

Dentro da função `main()` é onde colocamos as instruções que queremos que sejam lançadas no lançamento do programa.

Todo o codigo a executar tem de estar dentro `{ . . . }`

# Primiro Programa

```c
#include <stdio.h>

int main()
{
    return 0;
}
```

<br>

A saida deste programa seria um rendo vazio :)

C é conhecida por ser uma linguagem **case sensitive**, isto quer dizer que faz a diferenciação entre maiúsculas e minusculas.

A instrução `return 0` é um requisito da linguagem c. O unico objetivo é informar o sistema operativo que o programa terminou em problemas.

# Hello World 

```c
#include <stdio.h>

int main()
{
    printf("Hello World!");
    return 0;
}

```

<br>

Este é o habitual primeiro programa que escrevemos.

O output do programa é o seguinte:

![](assets/17645543159397.png)


A função que premite a escrita no ecrã é `printf`. Tratando-se de uma função esta tem necessariamente de ser ecrita com parênteses, assim: `printf(. . .)`. O que é acontece dentro dos parênteses é a comunicação com a função. Neste casso, passamos a string que é o conjunto de carateres delimitados por aspas que queremos que sejam escrta, ex: `printf("Hello World!")`

# #include <stdio.h>

A linguagem C não possui mecanismos de **input** e **output**.

Para solucionar este problema temos de recorrer a um conjnto de funções que existem em bibliotecas de funções disponibilizadas pela linguagem. 

Isto significa que adicionamos à linguagem um conjunto de outras funcionalidade que, por defeito ela não tem.

A linha `#include <stdio.h>` não é C, mas uma diretiva que indica ao compilador que deverá adicionar ao processo de compilação um ficheiro exeistente algures no disco do computado chamdo stdio.h.

<br>

| #include <stdio.h>             | Incluir as funções de input e output                             |
|--------------------------------|------------------------------------------------------------------|
| int main()                     | O Programa começa aqui                                           |
| {                              | Inicio do bloco de instruções                                    |
|        printf("Hello World!"); | Escrever a string "Hello World" usando a função printf           |
|        return 0;               | Terminar o programa e enviar o valor 0 para o sistema operativo. |
| }                              | Fim do bloco de instruções (e fim do programa )                  |


# \n

O `\n` serve para informar a função `printf` que a linha terminou e que é para mudar de linha.

`\n` significa new line.

O programa anterior ficaria assim:

```c
#include <stdio.h>

int main()
{
    printf("Hello World!"\n);
    return 0;
}

```
<br>

O resultado aparecerá assim:

 ![](assets/17645566843067.png)

# \

Quando quere-mos que o seguinte output seja apresentado:

> Hoje está uma "Lindo" dia !!!

Temos de usar `\` porque se não usarmos vai dar erro na compilação:

![](assets/17645620747511.png)

A forma correcta é a seguinte:

```c
#include <stdio.h>

int main()
{
    printf("Hoje está um \"LINDO\" dia!!!\n");
}
```
