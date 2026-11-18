# Resolução de Problemas e Desenvolvimento de Algoritmos

## 1. Introdução

A resolução de problemas e o desenvolvimento de algoritmos são fundamentos essenciais da Ciência da Computação e da programação.

Antes de escrever um programa, é necessário compreender o problema, identificar o que precisa ser resolvido, planejar uma solução e organizar os passos necessários para alcançar o resultado esperado.

Um computador não resolve problemas sozinho: ele executa instruções que foram desenvolvidas por um programador.

### Objetivos desta aula

Ao final desta aula, você deverá compreender:

- Como analisar e interpretar problemas.
- Como identificar entradas, processamento e saídas.
- Como desenvolver soluções passo a passo.
- O que são algoritmos.
- Como representar algoritmos.
- Como documentar soluções computacionais.
- Como transformar um algoritmo em um programa.

---

## 2. Análise e Solução de Problemas

A análise de problemas consiste em compreender uma situação e identificar o que precisa ser resolvido.

Na programação, essa etapa é muito importante porque escrever código sem entender o problema pode resultar em soluções incorretas ou incompletas.

### 2.1 Identificação do problema

O primeiro passo é entender exatamente qual é o problema.

É necessário responder a algumas perguntas:

- Qual é o problema?
- O que precisa ser calculado ou executado?
- Quais informações são necessárias?
- Qual resultado deve ser apresentado?
- Existem restrições ou condições?

**Exemplo:**

Imagine que precisamos desenvolver um programa que calcule a média de um aluno.

Primeiro, devemos compreender o problema:

- Precisamos receber duas notas.
- Precisamos somar as notas.
- Precisamos dividir o resultado por dois.
- Precisamos apresentar a média calculada.

### 2.2 Identificação das entradas, processamento e saídas

Um problema computacional geralmente pode ser dividido em três elementos fundamentais:

| Elemento | Descrição |
|---|---|
| Entrada (Input) | Dados fornecidos ao programa. |
| Processamento (Processing) | Operações realizadas com os dados. |
| Saída (Output) | Resultado produzido pelo programa. |

Esse modelo é conhecido como IPO (Input, Processing, Output).

**Exemplo: cálculo da média de duas notas.**

- **Entrada:** notas 8 e 6.
- **Processamento:** (8 + 6) / 2.
- **Saída:** 7.

### 2.3 Decomposição de problemas

A decomposição consiste em dividir um problema complexo em partes menores e mais simples.

**Exemplo: sistema de cadastro de alunos.**

Podemos dividir o sistema nas seguintes partes:

1. Cadastro de alunos.
2. Consulta de alunos.
3. Atualização de informações.
4. Exclusão de registros.
5. Emissão de relatórios.

### 2.4 Planejamento da solução

Depois de compreender o problema, precisamos planejar como resolvê-lo.

O planejamento envolve:

- Identificar os dados necessários.
- Definir as operações que serão realizadas.
- Estabelecer a sequência das instruções.
- Identificar possíveis condições.
- Verificar se a solução atende ao problema.

---

## 3. Algoritmos

Um algoritmo é uma sequência finita e organizada de instruções utilizadas para resolver um problema ou executar uma tarefa.

Os algoritmos estão presentes em diversas atividades do cotidiano.

**Exemplo: preparar um café.**

1. Pegar uma xícara.
2. Colocar água para aquecer.
3. Preparar o café.
4. Colocar o café na xícara.
5. Adicionar açúcar, se desejar.
6. Finalizar.

### 3.1 Características de um algoritmo

| Característica | Significado |
|---|---|
| Finitude | Deve possuir uma quantidade limitada de passos. |
| Clareza | As instruções devem ser compreensíveis. |
| Precisão | Cada instrução deve possuir um significado definido. |
| Efetividade | As operações devem poder ser executadas. |
| Entrada | Pode receber dados para realizar o processamento. |
| Saída | Deve produzir um resultado ou executar uma ação. |

### 3.2 Exemplo de algoritmo

Problema: calcular a soma de dois números.

**Algoritmo em linguagem natural:**

1. Iniciar.
2. Solicitar o primeiro número.
3. Solicitar o segundo número.
4. Somar os dois números.
5. Apresentar o resultado.
6. Finalizar.

**Representação em pseudocódigo:**

```text
Algoritmo "Soma"

    Declare numero1, numero2, resultado: inteiro

    Escreva("Digite o primeiro número:")
    Leia(numero1)

    Escreva("Digite o segundo número:")
    Leia(numero2)

    resultado <- numero1 + numero2

    Escreva("Resultado:", resultado)

FimAlgoritmo
```

**Implementação em C++:**

```cpp
#include <iostream>

using namespace std;

int main() {
    int numero1, numero2, resultado;

    cout << "Digite o primeiro numero: ";
    cin >> numero1;

    cout << "Digite o segundo numero: ";
    cin >> numero2;

    resultado = numero1 + numero2;

    cout << "Resultado: " << resultado << endl;

    return 0;
}
```

O algoritmo representa a lógica da solução, enquanto o código C++ implementa essa lógica utilizando uma linguagem de programação.

---

## 4. Representação de Algoritmos

A representação de algoritmos consiste em apresentar uma solução de maneira organizada para facilitar sua compreensão e implementação.

### 4.1 Linguagem natural

Consiste em descrever as instruções utilizando a linguagem humana.

**Exemplo: verificar se uma pessoa é maior de idade.**

```text
1. Iniciar.
2. Solicitar a idade da pessoa.
3. Verificar se a idade é maior ou igual a 18.
4. Se for, informar que é maior de idade.
5. Caso contrário, informar que é menor de idade.
6. Finalizar.
```

**Vantagem:** é simples e fácil de compreender.

**Desvantagem:** pode apresentar ambiguidades, principalmente em problemas complexos.

### 4.2 Pseudocódigo

O pseudocódigo é uma forma estruturada de representar algoritmos utilizando instruções semelhantes às linguagens de programação.

**Exemplo:**

```text
Algoritmo "Maioridade"

    Declare idade: inteiro

    Escreva("Digite sua idade:")
    Leia(idade)

    Se idade >= 18 Então
        Escreva("Maior de idade")
    Senão
        Escreva("Menor de idade")
    FimSe

FimAlgoritmo
```

**Vantagens:**

- Facilita o planejamento.
- Organiza a lógica.
- Não depende de uma linguagem específica.
- Facilita a conversão para código.

### 4.3 Fluxograma

Um fluxograma é uma representação gráfica de um algoritmo.

Ele utiliza símbolos geométricos para representar diferentes operações e decisões.

| Símbolo | Significado |
|---|---|
| Oval | Início ou fim. |
| Retângulo | Processamento. |
| Paralelogramo | Entrada ou saída de dados. |
| Losango | Decisão ou condição. |
| Seta | Direção do fluxo de execução. |

**Exemplo de fluxo lógico:**

```text
          (Início)
              |
              v
       [Receber idade]
              |
              v
        <Idade >= 18?>
           /       \
         SIM       NÃO
          |         |
          v         v
   [Maior de   [Menor de
     idade]      idade]
          \         /
           \       /
              v
             (Fim)
```

---

## 5. Documentação de Algoritmos

A documentação consiste em registrar informações sobre o funcionamento, a estrutura e a finalidade de um algoritmo ou programa.

### 5.1 Comentários no código

Comentários são textos adicionados ao código para explicar determinadas instruções.

**Comentário de uma linha:**

```cpp
// Calcula a soma de dois números
resultado = numero1 + numero2;
```

**Comentário de múltiplas linhas:**

```cpp
/*
    Programa responsável por calcular
    a soma de dois números inteiros.
*/

int resultado = numero1 + numero2;
```

Os comentários não são executados pelo programa.

### 5.2 Documentação da lógica

Além dos comentários, é importante documentar:

- Objetivo do algoritmo.
- Dados de entrada.
- Dados de saída.
- Variáveis utilizadas.
- Operações realizadas.
- Condições e regras.
- Possíveis limitações.

**Exemplo de documentação:**

```text
Nome: Calculadora de Soma

Objetivo:
Calcular a soma de dois números inteiros.

Entradas:
- Primeiro número.
- Segundo número.

Processamento:
Somar os dois números recebidos.

Saída:
Apresentar o resultado da soma.

Variáveis:
- numero1
- numero2
- resultado
```

### 5.3 Importância da documentação

1. Facilita a compreensão do código.
2. Ajuda na identificação de erros.
3. Facilita a manutenção do software.
4. Permite que outros desenvolvedores entendam o projeto.
5. Registra decisões tomadas durante o desenvolvimento.

---

## 6. Testes e Validação de Algoritmos

Depois de desenvolver um algoritmo, precisamos verificar se ele realmente resolve o problema.

Essa etapa é chamada de validação.

### 6.1 Teste de mesa

O teste de mesa consiste em executar manualmente as instruções de um algoritmo, acompanhando os valores das variáveis.

**Exemplo:**

```text
numero1 <- 10
numero2 <- 5

resultado <- numero1 + numero2

Escreva(resultado)
```

Tabela de execução:

| Etapa | numero1 | numero2 | resultado |
|---|---:|---:|---:|
| Inicialização | 10 | 5 | - |
| Soma | 10 | 5 | 15 |
| Saída | 10 | 5 | 15 |

Resultado esperado:

```text
15
```

### 6.2 Casos de teste

Um bom algoritmo deve ser testado com diferentes valores.

Exemplo: verificar se um número é positivo ou negativo.

| Entrada | Resultado esperado |
|---:|---|
| 10 | Positivo |
| -5 | Negativo |
| 0 | Zero |

---

## 7. Etapas do Desenvolvimento de Algoritmos

O desenvolvimento de algoritmos pode ser organizado em um processo com etapas bem definidas.

1. **Análise do problema:** compreender o problema e identificar o objetivo.
2. **Identificação dos dados:** definir as entradas, os processamentos e as saídas.
3. **Planejamento da solução:** organizar os passos necessários para resolver o problema.
4. **Representação do algoritmo:** utilizar linguagem natural, pseudocódigo ou fluxograma.
5. **Implementação:** transformar o algoritmo em código utilizando uma linguagem de programação.
6. **Testes e validação:** verificar se o programa produz os resultados esperados.
7. **Documentação e manutenção:** registrar o funcionamento e realizar melhorias quando necessário.

---

## 8. Exemplo Prático Completo

Vamos desenvolver um algoritmo para calcular a área de um retângulo.

### Etapa 1: Análise do problema

Precisamos calcular a área de um retângulo utilizando sua largura e altura.

### Etapa 2: Identificação das entradas e saídas

- Entrada: largura e altura.
- Processamento: multiplicação da largura pela altura.
- Saída: área do retângulo.

### Etapa 3: Fórmula matemática

```math
Área = largura \times altura
```

### Etapa 4: Pseudocódigo

```text
Algoritmo "AreaRetangulo"

    Declare largura, altura, area: real

    Escreva("Digite a largura:")
    Leia(largura)

    Escreva("Digite a altura:")
    Leia(altura)

    area <- largura * altura

    Escreva("Área do retângulo:", area)

FimAlgoritmo
```

### Etapa 5: Implementação em C++

```cpp
#include <iostream>

using namespace std;

int main() {
    double largura, altura, area;

    cout << "Digite a largura: ";
    cin >> largura;

    cout << "Digite a altura: ";
    cin >> altura;

    area = largura * altura;

    cout << "Area do retangulo: " << area << endl;

    return 0;
}
```

### Etapa 6: Teste

Considerando:

- Largura = 5
- Altura = 4

Aplicando a fórmula:

```text
Área = 5 * 4 = 20
```

Resultado:

```text
Area do retangulo: 20
```

---

## 9. Boas Práticas no Desenvolvimento de Algoritmos

- Entenda o problema antes de começar a programar.
- Divida problemas complexos em partes menores.
- Utilize nomes claros para as variáveis.
- Organize as instruções em uma sequência lógica.
- Evite operações desnecessárias.
- Utilize comentários quando forem úteis.
- Teste diferentes situações.
- Verifique se os resultados estão corretos.
- Mantenha a documentação atualizada.

---

## 10. Resumo da Aula

| Conceito | Definição |
|---|---|
| Análise de problemas | Processo de compreender e identificar o que precisa ser resolvido. |
| Decomposição | Divisão de problemas complexos em partes menores. |
| Algoritmo | Sequência finita e organizada de instruções. |
| Entrada | Dados fornecidos ao programa. |
| Processamento | Operações realizadas com os dados. |
| Saída | Resultado produzido pelo programa. |
| Pseudocódigo | Representação textual da lógica de um algoritmo. |
| Fluxograma | Representação gráfica de um algoritmo. |
| Documentação | Registro das informações sobre o funcionamento da solução. |
| Teste de mesa | Simulação manual da execução de um algoritmo. |

---

## 11. Conclusão

A resolução de problemas e o desenvolvimento de algoritmos são habilidades fundamentais para qualquer profissional da área de programação.

Antes de aprender a utilizar linguagens como C++, Python ou Java, é importante desenvolver o raciocínio lógico e compreender como transformar problemas em soluções organizadas.

Um bom programador não começa simplesmente escrevendo código. Ele primeiro entende o problema, planeja a solução, desenvolve o algoritmo, implementa e testa o resultado.

**A programação começa com a capacidade de pensar logicamente e organizar soluções.**

---

## 12. Exercícios para Fixação

### Questão 1

O que é um algoritmo?

a) Uma linguagem de programação.

b) Uma sequência organizada de instruções para resolver um problema.

c) Um componente físico do computador.

d) Um banco de dados.

### Questão 2

Quais são os três elementos do modelo IPO?

a) Código, compilação e execução.

b) Entrada, processamento e saída.

c) Hardware, software e usuário.

d) Variáveis, funções e classes.

### Questão 3

Qual é a finalidade de um fluxograma?

a) Representar graficamente um algoritmo.

b) Armazenar informações.

c) Compilar programas.

d) Criar bancos de dados.

### Questão 4

O que é decomposição de problemas?

a) Excluir partes de um programa.

b) Transformar código em linguagem natural.

c) Dividir um problema complexo em partes menores.

d) Executar um programa várias vezes.

### Questão 5

Para que serve o teste de mesa?

a) Instalar uma linguagem de programação.

b) Simular manualmente a execução de um algoritmo.

c) Criar interfaces gráficas.

d) Armazenar dados na memória.
