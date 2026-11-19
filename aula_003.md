# Estruturas de Programas: Decisão e Repetição

## 1. Introdução

Na programação, nem sempre um programa executa suas instruções em uma sequência simples, do início ao fim.

Muitas vezes, precisamos que o programa:

- Tome decisões dependendo de determinadas condições.
- Execute diferentes instruções conforme os valores recebidos.
- Repita determinadas operações várias vezes.
- Continue executando enquanto uma condição for verdadeira.

Para isso, utilizamos as **estruturas de controle de fluxo**.

Em C++, as estruturas de controle são divididas principalmente em três categorias:

1. **Sequência:** executa instruções na ordem em que foram escritas.
2. **Decisão (seleção):** permite escolher quais instruções serão executadas.
3. **Repetição (iteração):** permite executar instruções várias vezes.

Neste capítulo, estudaremos as estruturas de decisão e repetição.

---

## 2. Estruturas de Decisão

As estruturas de decisão permitem que um programa escolha diferentes caminhos durante sua execução.

Essa escolha acontece com base em uma condição lógica, que pode resultar em:

- `true`: verdadeiro.
- `false`: falso.

Em C++, as principais estruturas de decisão são:

- `if`
- `if else`
- `else if`
- `switch`

### 2.1 Estrutura if

A estrutura `if` permite executar um bloco de código somente quando determinada condição for verdadeira.

**Sintaxe**

```cpp
if (condicao) {
    // Código executado se a condição for verdadeira
}
```

**Exemplo**

```cpp
#include <iostream>
using namespace std;

int main() {
    int idade = 18;

    if (idade >= 18) {
        cout << "Maior de idade!" << endl;
    }

    return 0;
}
```

**Explicação**

1. Criamos uma variável chamada `idade`.
2. A estrutura `if` verifica se `idade` é maior ou igual a 18.
3. Como a condição é verdadeira, o programa executa o bloco de código.
4. A mensagem é exibida na tela.

Se a condição fosse falsa, o bloco seria ignorado.

### 2.2 Estrutura if else

A estrutura `if else` permite executar um bloco de código quando a condição é verdadeira e outro quando ela é falsa.

**Sintaxe**

```cpp
if (condicao) {
    // Executado se verdadeiro
} else {
    // Executado se falso
}
```

**Exemplo**

```cpp
#include <iostream>
using namespace std;

int main() {
    int numero = 7;

    if (numero % 2 == 0) {
        cout << "O numero e par." << endl;
    } else {
        cout << "O numero e impar." << endl;
    }

    return 0;
}
```

**Explicação:**

O operador `%` calcula o resto da divisão.

- Se o resto da divisão por 2 for zero, o número é par.
- Caso contrário, o número é ímpar.

### 2.3 Estrutura else if

A estrutura `else if` permite verificar várias condições diferentes.

Ela é útil quando precisamos escolher entre diversas possibilidades.

**Sintaxe**

```cpp
if (condicao1) {
    // Primeiro bloco
} else if (condicao2) {
    // Segundo bloco
} else if (condicao3) {
    // Terceiro bloco
} else {
    // Caso nenhuma condição seja verdadeira
}
```

**Exemplo**

```cpp
#include <iostream>
using namespace std;

int main() {
    int nota = 8;

    if (nota >= 9) {
        cout << "Excelente!" << endl;
    } else if (nota >= 7) {
        cout << "Aprovado!" << endl;
    } else if (nota >= 5) {
        cout << "Recuperacao!" << endl;
    } else {
        cout << "Reprovado!" << endl;
    }

    return 0;
}
```

**Explicação:**

O programa verifica as condições em sequência.

Assim que encontra uma condição verdadeira, executa o bloco correspondente e ignora os demais.

### 2.4 Estrutura switch

A estrutura `switch` permite selecionar um bloco de código com base no valor de uma expressão.

É bastante utilizada quando existem várias opções possíveis.

**Sintaxe**

```cpp
switch (variavel) {
    case valor1:
        // Código
        break;

    case valor2:
        // Código
        break;

    case valor3:
        // Código
        break;

    default:
        // Código executado se nenhum caso corresponder
}
```

**Exemplo**

```cpp
#include <iostream>
using namespace std;

int main() {
    int opcao = 2;

    switch (opcao) {
        case 1:
            cout << "Iniciar jogo" << endl;
            break;

        case 2:
            cout << "Configuracoes" << endl;
            break;

        case 3:
            cout << "Sair" << endl;
            break;

        default:
            cout << "Opcao invalida!" << endl;
    }

    return 0;
}
```

**Explicação:**

- `switch`: inicia a estrutura de seleção.
- `case`: representa uma possibilidade.
- `break`: encerra a execução do `switch`.
- `default`: executa quando nenhum caso corresponde ao valor.

**Importante:** sem `break`, a execução pode continuar para os próximos casos, comportamento conhecido como *fall-through*.

---

## 3. Estruturas de Repetição

As estruturas de repetição, também chamadas de laços ou loops, permitem executar um conjunto de instruções várias vezes.

Elas evitam que precisemos escrever repetidamente o mesmo código.

Em C++, existem três estruturas principais de repetição:

- for
- while
- do while

### 3.1 Estrutura for

A estrutura `for` é utilizada principalmente quando sabemos quantas vezes desejamos repetir uma operação.

**Sintaxe**

```cpp
for (inicializacao; condicao; incremento) {
    // Código que será repetido
}
```

A estrutura possui três partes:

1. **Inicialização:** define o valor inicial da variável de controle.
2. **Condição:** determina se a repetição deve continuar.
3. **Incremento:** atualiza a variável de controle.

**Exemplo**

```cpp
#include <iostream>
using namespace std;

int main() {

    for (int i = 1; i <= 5; i++) {
        cout << "Numero: " << i << endl;
    }

    return 0;
}
```

**Resultado:**

```text
Numero: 1
Numero: 2
Numero: 3
Numero: 4
Numero: 5
```

**Explicação:**

- `int i = 1`: começa a contagem em 1.
- `i <= 5`: continua enquanto `i` for menor ou igual a 5.
- `i++`: aumenta o valor de `i` em uma unidade.

### 3.2 Estrutura while

A estrutura `while` executa um bloco de código enquanto determinada condição for verdadeira.

Diferentemente do `for`, normalmente é utilizada quando não sabemos antecipadamente quantas repetições serão necessárias.

**Sintaxe**

```cpp
while (condicao) {
    // Código que será repetido
}
```

**Exemplo**

```cpp
#include <iostream>
using namespace std;

int main() {

    int contador = 1;

    while (contador <= 5) {
        cout << "Contador: " << contador << endl;

        contador++;
    }

    return 0;
}
```

**Resultado:**

```text
Contador: 1
Contador: 2
Contador: 3
Contador: 4
Contador: 5
```

**Explicação:**

1. Inicializamos o contador com o valor 1.
2. O `while` verifica se o contador é menor ou igual a 5.
3. Se a condição for verdadeira, executa o bloco.
4. O contador é incrementado.
5. O processo continua até a condição se tornar falsa.

**Atenção:** se a variável de controle não for atualizada corretamente, podemos criar um loop infinito.

### 3.3 Estrutura do while

A estrutura `do while` é semelhante ao `while`, mas possui uma diferença importante:

**O bloco de código é executado pelo menos uma vez, independentemente da condição.**

Isso acontece porque a condição é verificada somente depois da execução do bloco.

**Sintaxe**

```cpp
do {
    // Código executado
} while (condicao);
```

**Exemplo:**

```cpp
#include <iostream>
using namespace std;

int main() {

    int numero = 1;

    do {
        cout << "Numero: " << numero << endl;

        numero++;

    } while (numero <= 5);

    return 0;
}
```

**Resultado:**

```text
Numero: 1
Numero: 2
Numero: 3
Numero: 4
Numero: 5
```

**Diferença entre while e do while**

Observe o exemplo:

```cpp
int numero = 10;

while (numero < 5) {
    cout << "Executando while" << endl;
}
```

Nesse caso, nenhuma mensagem será exibida, pois a condição já começa falsa.

Agora:

```cpp
int numero = 10;

do {
    cout << "Executando do while" << endl;
} while (numero < 5);
```

Nesse caso, a mensagem será exibida uma vez, mesmo com a condição falsa.

---

## 4. Controle de Repetição

Além das estruturas de repetição, C++ possui instruções que permitem controlar o comportamento dos loops.

As principais são:

- `break`
- `continue`

### 4.1 Instrução break

A instrução `break` interrompe imediatamente a execução de um loop.

**Exemplo**

```cpp
#include <iostream>
using namespace std;

int main() {

    for (int i = 1; i <= 10; i++) {

        if (i == 5) {
            break;
        }

        cout << i << endl;
    }

    return 0;
}
```

**Resultado:**

```text
1
2
3
4
```

Quando `i` chega a `5`, o `break` encerra o loop.

### 4.2
