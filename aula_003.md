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
2. 
