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
