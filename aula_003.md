# Ciência da Computação — Aula 3

## Lógica de Programação e Algoritmos

## 1. Introdução à Lógica de Programação

A **Lógica de Programação** é a área que estuda como organizar pensamentos e instruções de maneira lógica para resolver problemas utilizando computadores.

Antes de desenvolver um programa, é necessário compreender o problema, identificar quais informações serão utilizadas e determinar quais passos devem ser executados para alcançar o resultado desejado.

A lógica de programação é a base para aprender qualquer linguagem de programação, como:

- C
- C++
- Java
- Python
- JavaScript
- C#

Independentemente da linguagem utilizada, os fundamentos da lógica de programação permanecem praticamente os mesmos.

### 1.1 Por que aprender Lógica de Programação?

Aprender lógica de programação é importante porque permite:

- Desenvolver raciocínio lógico.
- Resolver problemas de maneira organizada.
- Criar algoritmos.
- Compreender como os programas funcionam.
- Identificar erros na execução de programas.
- Desenvolver soluções computacionais.
- Aprender diferentes linguagens de programação com mais facilidade.

---

## 2. O que é Raciocínio Lógico?

O **raciocínio lógico** é a capacidade de analisar informações, identificar relações e chegar a conclusões por meio de regras e deduções.

Na programação, utilizamos o raciocínio lógico para determinar quais instruções precisam ser executadas para resolver determinado problema.

### 2.1 Exemplo prático

Imagine o seguinte problema:

Uma pessoa deseja descobrir se um número é par ou ímpar.

Para resolver esse problema, precisamos estabelecer uma regra:

- Se o número for divisível por 2, ele é par.
- Caso contrário, ele é ímpar.

Podemos representar essa lógica da seguinte maneira:

```text
INÍCIO

    Ler um número

    Se o número for divisível por 2
        Mostrar "Número par"
    Senão
        Mostrar "Número ímpar"

FIM
```

Essa sequência representa uma solução lógica para o problema.

---

## 3. O que é Pensamento Computacional?

O **Pensamento Computacional** é uma forma de organizar o raciocínio para resolver problemas utilizando conceitos fundamentais da computação.

Ele não é utilizado apenas por programadores, mas também pode ser aplicado em situações do cotidiano.

O pensamento computacional possui quatro pilares principais:

### 3.1 Decomposição

Consiste em dividir um problema complexo em partes menores e mais simples.

**Exemplo:**

Criar um sistema de gerenciamento de uma biblioteca.

Podemos dividir o projeto em:

- Cadastro de livros.
- Cadastro de usuários.
- Empréstimos.
- Devoluções.
- Consultas ao acervo.

Cada parte pode ser desenvolvida separadamente.

### 3.2 Reconhecimento de Padrões

Consiste em identificar características ou comportamentos que se repetem em diferentes problemas.

**Exemplo:**

Imagine que precisamos calcular a média de vários alunos.

Todos os cálculos seguem a mesma estrutura:

1. Receber as notas.
2. Somar as notas.
3. Dividir pela quantidade de notas.
4. Apresentar a média.

Identificar esse padrão permite criar uma solução que pode ser reutilizada.

### 3.3 Abstração

Consiste em identificar as informações importantes de um problema e ignorar detalhes que não são necessários para sua resolução.

**Exemplo:**

Ao desenvolver um sistema de cadastro de alunos, podemos utilizar informações como:

- Nome.
- Idade.
- Matrícula.
- Curso.

Não precisamos armazenar informações que não possuem relação com o objetivo do sistema.

### 3.4 Algoritmos

Consiste em organizar uma sequência de instruções para resolver um problema.

**Exemplo:**

```text
INÍCIO

    Ler dois números
    Somar os números
    Mostrar o resultado

FIM
```

### Resumo dos quatro pilares

| Pilar | Descrição |
|---|---|
| Decomposição | Dividir problemas em partes menores |
| Reconhecimento de padrões | Identificar elementos repetidos |
| Abstração | Selecionar informações importantes |
| Algoritmos | Organizar instruções para resolver problemas |

---

## 4. O que é um Algoritmo?

Um **algoritmo** é uma sequência finita, organizada e lógica de instruções utilizadas para resolver um problema ou executar uma tarefa.

Os algoritmos estão presentes em praticamente todas as atividades realizadas por computadores.

Entretanto, eles também podem representar tarefas do cotidiano.

### 4.1 Exemplo de Algoritmo no Cotidiano

Problema: preparar um sanduíche.

```text
INÍCIO

    Pegar duas fatias de pão

    Colocar queijo sobre uma fatia

    Colocar presunto sobre o queijo

    Cobrir com a outra fatia de pão

    Servir o sanduíche

FIM
```

Esse exemplo representa um algoritmo porque apresenta uma sequência organizada de instruções para alcançar um objetivo.

### 4.2 Características de um Algoritmo

Um algoritmo deve apresentar algumas características importantes:

**1. Finitude**

Deve possuir uma quantidade limitada de etapas e terminar após sua execução.

**2. Clareza**

As instruções devem ser compreensíveis e não apresentar ambiguidades.

**3. Precisão**

Cada instrução deve indicar claramente o que precisa ser realizado.

**4. Entrada**

Pode receber dados necessários para resolver determinado problema.

**5. Saída**

Deve produzir algum resultado ou efeito esperado.

**6. Efetividade**

As operações devem ser executáveis e capazes de contribuir para a resolução do problema.

---

## 5. Formas de Representar Algoritmos

Existem diferentes maneiras de representar algoritmos antes de transformá-los em programas.

As três formas mais conhecidas são:

- Descrição narrativa.
- Pseudocódigo.
- Fluxograma.

### 5.1 Descrição Narrativa

A descrição narrativa utiliza linguagem natural para explicar as etapas de um algoritmo.

**Exemplo: calcular a soma de dois números.**

1. Solicitar o primeiro número.
2. Solicitar o segundo número.
3. Somar os dois números.
4. Apresentar o resultado.

Essa representação é simples e fácil de compreender.

Entretanto, algoritmos muito grandes podem ficar difíceis de organizar utilizando apenas textos.

### 5.2 Pseudocódigo

O **pseudocódigo** é uma forma de representar algoritmos utilizando uma linguagem estruturada semelhante à programação.

Ele não depende de uma linguagem de programação específica.

**Exemplo:**

```text
Algoritmo "Soma"

Var
    numero1, numero2, resultado: inteiro

Inicio

    Escreva("Digite o primeiro número:")
    Leia(numero1)

    Escreva("Digite o segundo número:")
    Leia(numero2)

    resultado <- numero1 + numero2

    Escreva("Resultado:", resultado)

Fim
```

O pseudocódigo facilita a compreensão da lógica antes da implementação em uma linguagem de programação.

### 5.3 Fluxograma

Um **fluxograma** é uma representação visual de um algoritmo.

Ele utiliza símbolos geométricos conectados por setas para demonstrar a sequência de execução das instruções.

Os principais símbolos são:

| Símbolo | Nome | Função |
|---|---|---|
| Oval | Terminal | Representa início e fim |
| Retângulo | Processo | Representa operações |
| Losango | Decisão | Representa condições |
| Paralelogramo | Entrada/Saída | Representa leitura e apresentação de dados |
| Seta | Linha de fluxo | Indica a direção da execução |

**Exemplo: verificar se um número é positivo.**

```text
          INÍCIO
             |
             v
       Ler um número
             |
             v
       Número > 0?
          /     \
        Sim     Não
         |       |
         v       v
     "Positivo" "Não positivo"
         |       |
         \       /
          \     /
             |
             v
             FIM
```

---

## 6. Variáveis

Uma **variável** é um espaço identificado na memória utilizado para armazenar um valor que pode ser alterado durante a execução de um programa.

As variáveis permitem armazenar informações que serão utilizadas posteriormente.

### 6.1 Exemplo de Variável

Imagine um programa que precisa armazenar a idade de uma pessoa.

```text
idade = 20
```

Nesse exemplo:

- `idade` é o nome da variável.
- `20` é o valor armazenado.

O valor de uma variável pode ser modificado durante a execução do programa.

**Exemplo:**

```text
idade = 20

idade = 25
```

Após a segunda atribuição, o valor armazenado será `25`.

### 6.2 Regras para Nomear Variáveis

Os nomes das variáveis devem seguir determinadas regras, que podem variar conforme a linguagem de programação.

Boas práticas:

- Utilizar nomes significativos.
- Não começar o nome com números.
- Evitar espaços.
- Não utilizar palavras reservadas da linguagem.
- Preferir nomes que indiquem a finalidade da variável.

**Exemplos válidos:**

```text
idade
nome
salario
numeroAluno
totalCompra
```

**Exemplos inválidos em linguagens como C++:**

```text
2idade
nome completo
int
```

---

## 7. Constantes

Uma **constante** é um identificador utilizado para armazenar um valor que não deve ser modificado durante a execução do programa.

Diferentemente das variáveis, as constantes representam valores fixos.

### 7.1 Exemplo de Constante

```text
PI = 3.14159
```

O valor de PI representa uma constante matemática.

Em C++, podemos declarar uma constante utilizando a palavra-chave `const`.

**Exemplo em C++:**

```cpp
#include <iostream>

int main() {

    const double PI = 3.14159;

    std::cout << PI;

    return 0;
}
```

O programa apresenta o valor da constante na tela.

### 7.2 Diferença entre Variáveis e Constantes

| Variável | Constante |
|---|---|
| Pode ter seu valor alterado | Não pode ter seu valor alterado após a inicialização |
| Armazena valores modificáveis | Armazena valores fixos |
| Exemplo: idade | Exemplo: PI |

---

## 8. Tipos de Dados

Os **tipos de dados** definem quais tipos de valores podem ser armazenados em uma variável.

Cada linguagem de programação possui seus próprios tipos de dados e regras de utilização.

Os tipos mais comuns são:

### 8.1 Inteiros (Integer)

Utilizados para armazenar números inteiros, positivos, negativos ou zero.

Exemplos:

```text
10
-5
0
150
```

Em C++:

```cpp
int idade = 20;
```

### 8.2 Reais (Float / Double)

Utilizados para armazenar números com casas decimais.

Exemplos:

```text
10.5
3.14
-2.75
```

Em C++:

```cpp
float altura = 1.75f;

double salario = 2500.50;
```

### 8.3 Caracteres (Char)

Utilizados para armazenar um único caractere.

Exemplos:

```text
'A'
'B'
'Z'
'7'
```

Em C++:

```cpp
char letra = 'A';
```

### 8.4 Cadeias de Caracteres (String)

Utilizadas para armazenar sequências de caracteres, como nomes, frases e textos.

Em C++:

```cpp
#include <string>

std::string nome = "Carlos";
```

### 8.5 Booleanos (Boolean)

Utilizados para representar valores lógicos.

Existem apenas dois valores possíveis:

- `true`: verdadeiro.
- `false`: falso.

Em C++:

```cpp
bool aprovado = true;
```

### 8.6 Tabela de Tipos de Dados

| Tipo | Descrição | Exemplo |
|---|---|---|
| int | Números inteiros | 25 |
| float | Números decimais | 10.5f |
| double | Números decimais com maior precisão | 3.14159 |
| char | Um caractere | 'A' |
| string | Texto | "Olá" |
| bool | Valores lógicos | true |

---

## 9. Operadores

Os **operadores** são símbolos utilizados para realizar operações sobre valores e variáveis.

Na programação, existem diferentes categorias de operadores.

### 9.1 Operadores Aritméticos

São utilizados para realizar operações matemáticas.

| Operador | Operação | Exemplo |
|---|---|---|
| + | Adição | 10 + 5 |
| - | Subtração | 10 - 5 |
| * | Multiplicação | 10 * 5 |
| / | Divisão | 10 / 5 |
| % | Resto da divisão | 10 % 3 |

**Exemplo em C++:**

```cpp
#include <iostream>

int main() {

    int a = 10;
    int b = 5;

    std::cout << a + b << "\n";
    std::cout << a - b << "\n";
    std::cout << a * b << "\n";
    std::cout << a / b << "\n";

    return 0;
}
```

Resultado:

```text
15
5
50
2
```

### 9.2 Operadores Relacionais

São utilizados para comparar valores.

O resultado de uma comparação é um valor booleano: verdadeiro ou falso.

| Operador | Significado |
|---|---|
| == | Igual a |
| != | Diferente de |
| > | Maior que |
| < | Menor que |
| >= | Maior ou igual |
| <= | Menor ou igual |

**Exemplo em C++:**

```cpp
int idade = 20;

bool resultado = idade >= 18;
```

Nesse exemplo, o resultado será `true`, pois 20 é maior ou igual a 18.

### 9.3 Operadores Lógicos

São utilizados para combinar ou modificar expressões lógicas.

| Operador | Significado |
|---|---|
| && | E lógico (AND) |
| \|\| | OU lógico (OR) |
| ! | NÃO lógico (NOT) |

**Exemplo em C++:**

```cpp
int idade = 20;
bool possuiDocumento = true;

bool podeEntrar = idade >= 18 && possuiDocumento;
```

A variável `podeEntrar` receberá `true` porque as duas condições são verdadeiras.

---

## 10. Entrada e Saída de Dados

Os programas precisam receber informações e apresentar resultados.

Essas operações são conhecidas como entrada e saída de dados.

### 10.1 Entrada de Dados

A entrada de dados consiste em receber informações do usuário ou de outra fonte.

Em C++, podemos utilizar `std::cin` para receber dados pelo teclado.

**Exemplo:**

```cpp
#include <iostream>

int main() {

    int idade;

    std::cout << "Digite sua idade: ";
    std::cin >> idade;

    return 0;
}
```

### 10.2 Saída de Dados

A saída de dados consiste em apresentar informações ao usuário.

Em C++, utilizamos `std::cout`.

**Exemplo:**

```cpp
#include <iostream>

int main() {

    std::cout << "Bem-vindo ao programa!";

    return 0;
}
```

### 10.3 Entrada e Saída Combinadas

Podemos utilizar entrada e saída para criar programas interativos.

**Exemplo:**

```cpp
#include <iostream>

int main() {

    int numero;

    std::cout << "Digite um numero: ";
    std::cin >> numero;

    std::cout << "Voce digitou: " << numero;

    return 0;
}
```

---

## 11. Estruturas Básicas de um Algoritmo

Um algoritmo pode utilizar três estruturas fundamentais para controlar sua execução:

1. Sequência.
2. Decisão.
3. Repetição.

### 11.1 Estrutura Sequencial

A estrutura sequencial executa instruções uma após a outra, seguindo a ordem em que foram escritas.

**Exemplo:**

```text
INÍCIO

    Ler primeiro número

    Ler segundo número

    Somar os números

    Mostrar resultado

FIM
```

### 11.2 Estrutura de Decisão

A estrutura de decisão permite executar diferentes instruções dependendo de uma condição.

**Exemplo:**

```text
INÍCIO

    Ler idade

    SE idade >= 18 ENTÃO

        Mostrar "Maior de idade"

    SENÃO

        Mostrar "Menor de idade"

    FIM SE

FIM
```

### 11.3 Estrutura de Repetição

A estrutura de repetição permite executar um conjunto de instruções várias vezes.

**Exemplo:**

```text
INÍCIO

    PARA contador DE 1 ATÉ 5 FAÇA

        Mostrar contador

    FIM PARA

FIM
```

Resultado:

```text
1
2
3
4
5
```

---

## 12. Resolução de Problemas Utilizando Algoritmos

A programação consiste principalmente em transformar problemas em soluções computacionais.

Para isso, podemos seguir algumas etapas:

1. Identificar o problema.
2. Analisar as informações disponíveis.
3. Identificar os dados de entrada.
4. Definir as operações necessárias.
5. Elaborar o algoritmo.
6. Testar a solução.
7. Implementar o algoritmo em uma linguagem de programação.

### 12.1 Exemplo: Calcular a Média de um Aluno

**Problema:**

Criar um algoritmo que receba duas notas de um aluno, calcule a média e apresente o resultado.

**Etapa 1 — Identificar as entradas**

- Primeira nota.
- Segunda nota.

**Etapa 2 — Definir o processamento**

Somar as notas e dividir por dois.

**Etapa 3 — Definir a saída**

Apresentar a média calculada.

**Algoritmo em pseudocódigo:**

```text
INÍCIO

    Ler nota1

    Ler nota2

    media <- (nota1 + nota2) / 2

    Mostrar media

FIM
```

**Implementação em C++:**

```cpp
#include <iostream>

int main() {

    double nota1;
    double nota2;
    double media;

    std::cout << "Digite a primeira nota: ";
    std::cin >> nota1;

    std::cout << "Digite a segunda nota: ";
    std::cin >> nota2;

    media = (nota1 + nota2) / 2;

    std::cout << "Media: " << media << "\n";

    return 0;
}
```

---

## 13. Erros em Algoritmos e Programas

Durante o desenvolvimento de algoritmos e programas, podem ocorrer erros.

Os três tipos mais comuns são:

### 13.1 Erros de Sintaxe

Ocorrem quando as regras da linguagem de programação são desrespeitadas.

**Exemplo em C++:**

```cpp
#include <iostream>

int main() {

    std::cout << "Ola, mundo!"

    return 0;
}
```

Nesse exemplo, falta um ponto e vírgula após a instrução `std::cout`.

### 13.2 Erros de Execução

Ocorrem enquanto o programa está sendo executado.

Podem acontecer por diferentes motivos, como operações inválidas ou acesso a recursos indisponíveis.

### 13.3 Erros de Lógica

Ocorrem quando o programa executa, mas produz um resultado diferente do esperado.

**Exemplo:**

```cpp
int a = 10;
int b = 5;

int resultado = a - b;
```

Se o objetivo era somar os números, o operador utilizado está incorreto.

O programa pode executar normalmente, mas produzir um resultado errado.

---

## 14. Importância da Lógica de Programação

A lógica de programação é uma das habilidades mais importantes para quem deseja trabalhar com desenvolvimento de software.

Ela permite:

- Desenvolver soluções organizadas.
- Compreender algoritmos.
- Criar programas eficientes.
- Identificar e corrigir erros.
- Desenvolver raciocínio computacional.
- Aprender diferentes linguagens.
- Resolver problemas de maneira estruturada.

Dominar esses conceitos facilita o aprendizado de linguagens como C++, Python, Java e JavaScript.

---

## 15. Resumo da Aula

Nesta aula, estudamos:

1. Introdução à lógica de programação.
2. Raciocínio lógico.
3. Pensamento computacional.
4. Os quatro pilares do pensamento computacional.
5. Conceito de algoritmo.
6. Características de um algoritmo.
7. Descrição narrativa.
8. Pseudocódigo.
9. Fluxogramas.
10. Variáveis.
11. Constantes.
12. Tipos de dados.
13. Operadores aritméticos.
14. Operadores relacionais.
15. Operadores lógicos.
16. Entrada e saída de dados.
17. Estruturas sequenciais, condicionais e de repetição.
18. Resolução de problemas.
19. Erros de sintaxe, execução e lógica.

---

## 16. Exercícios de Fixação

### Questões Teóricas

**1.** O que é lógica de programação?

**2.** Qual é a importância do raciocínio lógico na programação?

**3.** O que é pensamento computacional?

**4.** Quais são os quatro pilares do pensamento computacional?

**5.** O que é um algoritmo?

**6.** Quais são as principais características de um algoritmo?

**7.** Qual é a diferença entre descrição narrativa e pseudocódigo?

**8.** O que é um fluxograma?

**9.** Qual é a diferença entre variável e constante?

**10.** O que são tipos de dados?

**11.** Qual é a diferença entre os tipos `int`, `float`, `char` e `bool`?

**12.** Para que servem os operadores aritméticos?

**13.** Qual é a diferença entre operadores relacionais e operadores lógicos?

**14.** Qual é a finalidade das estruturas de decisão?

**15.** O que são estruturas de repetição?

**16.** Qual é a diferença entre erros de sintaxe e erros de lógica?

### Exercícios Práticos

**17.** Crie um algoritmo que receba dois números e apresente a soma.

**18.** Crie um algoritmo que receba um número e informe se ele é par ou ímpar.

**19.** Crie um algoritmo que receba a idade de uma pessoa e informe se ela é maior ou menor de idade.

**20.** Crie um algoritmo que receba três notas e calcule a média.

**21.** Crie um algoritmo que receba dois números e apresente o maior deles.

**22.** Crie um algoritmo que apresente os números de 1 até 10 utilizando uma estrutura de repetição.

---

## 17. Próxima Aula

# Aula 4 — Introdução à Programação

Conteúdos que serão estudados:

- O que é programação?
- Linguagens de programação.
- Linguagens de baixo e alto nível.
- Linguagens compiladas e interpretadas.
- Compiladores.
- Interpretadores.
- Código-fonte.
- Código de máquina.
- Processo de compilação.
- Introdução à linguagem C++.
- Estrutura básica de um programa.
- Primeiro programa em C++.

---

*Fim da Aula 3 — Lógica de Programação e Algoritmos.*
