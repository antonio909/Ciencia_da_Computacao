# Tipos de Dados Simples

Os **tipos de dados simples** são utilizados para armazenar informações básicas em um programa, como números inteiros, números decimais, caracteres e valores lógicos.

Em C++, cada variável precisa ter um tipo de dado definido, que determina quais valores ela pode armazenar e quais operações podem ser realizadas com ela.

## 1. O que são tipos de dados?

Um tipo de dado (Data Type) define a natureza da informação que uma variável pode armazenar.

Por exemplo:

 ```cpp
int idade = 18;
float altura = 1.75;
char inicial = 'A';
bool aprovado = true;
```

Nesse exemplo, temos quatro variáveis com diferentes tipos de dados.

## 2. Principais tipos de dados simples

C++ possui diversos tipos de dados fundamentais.

| Tipo | Descrição | Exemplo |
|---|---|---|
| `int` | Números inteiros | `10` |
| `float` | Números decimais | `3.14f` |
| `double` | Números decimais com maior precisão | `3.141592` |
| `char` | Um único caractere | `'A'` |
| `bool` | Valores lógicos | `true` ou `false` |
| `void` | Ausência de valor | — |

### 2.1 int (Integer)

O tipo `int` é utilizado para armazenar números inteiros, positivos, negativos ou zero.

Exemplo:

```cpp
#include <iostream>
using namespace std;

int main() {
    int idade = 20;
    int temperatura = -5;
    int quantidade = 100;

    cout << idade << endl;
    cout << temperatura << endl;
    cout << quantidade << endl;

    return 0;
}
```

### 2.2 float

O tipo `float` é utilizado para armazenar números com casas decimais.

Exemplo:

```cpp
#include <iostream>
using namespace std;

int main() {
    float altura = 1.75f;
    float temperatura = 36.5f;

    cout << altura << endl;
    cout << temperatura << endl;

    return 0;
}
```

O sufixo `f` indica que o valor literal é do tipo `float`.

### 2.3. double

O tipo `double` também armazena números decimais, mas oferece maior precisão do que `float`.

Exemplo:

```cpp
#include <iostream>
using namespace std;

int main() {
    double pi = 3.141592653589793;
    double distancia = 1234.56789;

    cout << pi << endl;
    cout << distancia << endl;

    return 0;
}
```

**Diferença entre float e double:**

| Característica | float | double |
|---|---|---|
| Tamanho típico | 4 bytes | 8 bytes |
| Precisão aproximada | 6 a 7 dígitos | 15 a 16 dígitos |
| Precisão | Menor | Maior |

### 2.4. char (Character)

O tipo `char` é utilizado para armazenar um único caractere.

Os caracteres são representados entre aspas simples.

Exemplo:

```cpp
#include <iostream>
using namespace std;

int main() {
    char letra = 'A';
    char simbolo = '#';
    char numero = '7';

    cout << letra << endl;
    cout << simbolo << endl;
    cout << numero << endl;

    return 0;
}
```

Importante: `'7'` é um caractere, enquanto `7` é um número inteiro.

### 2.5. bool (Boolean)

O tipo `bool` representa valores lógicos e possui apenas dois estados:

- `true`: verdadeiro.
- `false`: falso.

Exemplo:

```cpp
#include <iostream>
using namespace std;

int main() {
    bool aprovado = true;
    bool reprovado = false;

    cout << aprovado << endl;
    cout << reprovado << endl;

    return 0;
}
```

Por padrão, o C++ apresenta `true` como `1` e `false` como `0` quando são enviados diretamente ao `cout`.

### 2.6. void

O tipo `void` representa a ausência de um valor.

É utilizado principalmente em funções que não retornam nenhum resultado.

Exemplo:

```cpp
#include <iostream>
using namespace std;

void mensagem() {
    cout << "Ola, mundo!" << endl;
}

int main() {
    mensagem();

    return 0;
}
```

A função `mensagem()` utiliza `void` porque não retorna nenhum valor.

## 3. Modificadores de tipos

C++ permite modificar alguns tipos fundamentais para alterar sua capacidade de armazenamento ou representação.

Os principais modificadores são:

| Modificador | Descrição |
|---|---|
| `signed` | Permite valores positivos e negativos. |
| `unsigned` | Permite apenas valores não negativos.
| `short` | Define um tipo inteiro de menor capacidade, quando disponível. |
| `long` | Define um tipo inteiro ou decimal de maior capacidade, conforme o tipo utilizado. |

Exemplo:

```cpp
#include <iostream>
using namespace std;

int main() {
    short numero1 = 100;
    long numero2 = 1000000;
    unsigned int numero3 = 500;
    signed int numero4 = -100;

    cout << numero1 << endl;
    cout << numero2 << endl;
    cout << numero3 << endl;
    cout << numero4 << endl;

    return 0;
}
```

## 4. Descobrindo o tamanho dos tipos de dados
