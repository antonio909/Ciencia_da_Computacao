# Conceitos Básicos sobre Computadores

## 1. Introdução

O computador é uma máquina eletrônica capaz de receber, processar, armazenar e transmitir informações. Ele executa instruções fornecidas por programas para realizar diferentes tarefas.

Atualmente, os computadores estão presentes em praticamente todas as áreas da sociedade, como educação, medicina, engenharia, comunicação, entretenimento e desenvolvimento de softwares.

Para compreender como um computador funciona e como desenvolver programas, precisamos conhecer alguns conceitos fundamentais:

- Hardware
- Software
- Sistema Operacional
- Compiladores
- Representação Interna de Dados
- Linguagem de Programação.

---

## 2. Hardware

**O que é Hardware?**

Hardware é o conjunto de componentes físicos de um computador, ou seja, todas as partes que podemos tocar.

Esses componentes são responsáveis por executar operações, armazenar informações, receber dados e apresentar resultados.

**Principais componentes de Hardware**

### 2.1 Processador (CPU)

A CPU (Central Processing Unit), também conhecida como Unidade Central de Processamento, é responsável por executar instruções e realizar operações matemáticas e lógicas.

É considerada um dos principais componentes do computador.

Suas principais funções são:

- Executar instruções dos programas.
- Realizar cálculos matemáticos.
- Executar operações lógicas.
- Coordenar operações entre componentes.

A CPU possui algumas partes importantes:

- **Unidade de Controle (UC):** coordena a execução das instruções.
- **Unidade Lógica e Aritmética (ULA):** realiza operações matemáticas e lógicas.
- **Registradores:** pequenas áreas de armazenamento extremamente rápidas dentro do processador.

### 2.2 Memória RAM

RAM significa Random Access Memory (Memória de Acesso Aleatório).

É responsável por armazenar temporariamente os dados e programas que estão sendo utilizados pelo computador.

Características:

- Armazenamento temporário.
- Permite acesso rápido aos dados.
- Perde as informações quando o computador é desligado.
- Quanto maior sua capacidade, mais dados e programas podem permanecer disponíveis simultaneamente.

### 2.3 Armazenamento (HD e SSD)

São dispositivos responsáveis por armazenar permanentemente arquivos, programas e o sistema operacional.

Existem dois tipos bastante conhecidos:

**HD (Hard Disk):**

- Utiliza discos magnéticos.
- Possui partes mecânicas.
- Geralmente apresenta menor velocidade que um SSD.

**SSD (Solid State Drive):**

- Utiliza memória flash.
- Não possui partes mecânicas móveis.
- Geralmente oferece velocidades maiores de leitura e gravação.

### 2.4 Placa-mãe

A placa-mãe é a principal placa de circuitos do computador.

Ela conecta os componentes e permite a comunicação entre eles.

Nela são conectados:

- Processador.
- Memória RAM.
- Dispositivos de armazenamento.
- Placa de vídeo.
- Placas de expansão.

### 2.5 Dispositivos de Entrada e Saída

Os dispositivos de entrada permitem enviar informações para o computador.

Exemplos:

- Teclado.
- Mouse.
- Microfone.
- Scanner.
- Webcam.

Os dispositivos de saída permitem apresentar informações processadas pelo computador.

Exemplos:

- Monitor.
- Impressora.
- Alto-falantes.
- Fones de ouvido.

---

## 3. Software

**O que é Software?**

Software é o conjunto de programas, instruções e dados que orientam o funcionamento de um computador.

Diferente do hardware, o software não é físico. Ele representa a parte lógica do sistema computacional.

Sem software, o hardware não teria instruções para executar tarefas específicas.

**Tipos de Software**

### 3.1 Software de Sistema

São programas responsáveis por controlar e gerenciar o funcionamento do computador.

Exemplos:

- Windows.
- Linux.
- macOS.
- Drivers de dispositivos.

### 3.2 Software Aplicativo

São programas desenvolvidos para ajudar os usuários a realizar tarefas específicas.

Exemplos:

- Google Chrome.
- Microsoft Word.
- Photoshop.
- VLC Media Player.
- Jogos eletrônicos.

### 3.3 Software de Programação

São ferramentas utilizadas pelos desenvolvedores para criar outros programas.

Exemplos:

- Compiladores.
- Interpretadores.
- Editores de código.
- Depuradores (Debuggers).
- Ambientes de desenvolvimento integrados (IDEs).

---

## 4. Sistema Operacional

**O que é um Sistema Operacional?**

O Sistema Operacional (SO) é um software responsável por gerenciar os recursos do computador e permitir a interação entre o usuário, os programas e o hardware.

Ele funciona como uma camada intermediária entre os aplicativos e os componentes físicos.

**Principais funções de um Sistema Operacional**

**1. Gerenciamento de Processos**

Controla os programas que estão sendo executados no computador.

**2. Gerenciamento de Memória**

Controla a utilização da memória RAM pelos programas.

**3. Gerenciamento de Arquivos**

Organiza arquivos e diretórios, permitindo criar, modificar, copiar e excluir informações.

**4. Gerenciamento de Dispositivos**

Controla a comunicação com dispositivos como teclado, mouse, impressora e armazenamento.

**5. Interface com o Usuário**

Permite que o usuário interaja com o computador por meio de interfaces gráficas ou linhas de comando.

**Exemplos de Sistemas Operacionais**

- **Windows:** sistema operacional desenvolvido pela Microsoft.
- **Linux:** família de sistemas operacionais de código aberto.
- **macOS:** sistema operacional dos computadores Mac.
- **Android:** sistema operacional utilizado em diversos dispositivos móveis.
- **iOS:** sistema operacional utilizado em dispositivos móveis da Apple.

---

## 5. Compiladores

**O que é um Compilador?**

Um compilador é um programa responsável por traduzir o código-fonte escrito em uma linguagem de programação para uma representação que possa ser executada ou utilizada por outras ferramentas.

Os computadores executam instruções em linguagem de máquina, enquanto os programadores geralmente escrevem códigos em linguagens de alto nível, como C, C++ e Java.

O compilador realiza a tradução entre essas representações.

**Como funciona a compilação?**

**Etapas principais:**

 1. **Código-fonte:** código escrito pelo programador.
 2. **Compilação:** tradução do código para uma representação de nível mais baixo.
 3. **Código-objeto:** resultado intermediário da compilação.
 4. **Linkedição:** combinação dos arquivos necessários e bibliotecas.
 5. **Executável:** programa pronto para ser executado, conforme a plataforma.

**Exemplo em C++**

```cpp
#include <iostream>

int main() {
    std::cout << "Hello, World!" << std::endl;

    return 0;
}
```

Para compilar esse programa utilizando o compilador GCC ou G++:

```bash
g++ main.cpp -o programa
```

Para executar no Windows:

```powershell
.\programa.exe
```

O compilador transforma o código-fonte em um executável que pode ser executado pelo sistema operacional.

**Compilador vs Interpretador**

| Compilador | Interpretador |
|---|---|
| Traduz o programa antes da execução, conforme o modelo utilizado. | Executa instruções por meio de um processo de interpretação. |
| Pode gerar um executável independente. | Geralmente depende de um ambiente de execução. |
| Exemplo: GCC e Clang. | Exemplo: interpretador Python. |

Observação: existem linguagens e ambientes que combinam compilação, interpretação e compilação durante a execução (JIT).

---

## 6. Representação Interna de Dados

**Como o computador representa informações?**

Os computadores utilizam sinais elétricos para representar informações internamente.

Essas informações são representadas por meio de dois estados fundamentais:

- 0 (zero).
- 1 (um).

Esse sistema é conhecido como sistema binário.

Cada dígito binário é chamado de **bit** (Binary Digit).

### 6.1 Bit e Byte

**Bit:** menor unidade de informação digital, podendo assumir os valores 0 ou 1.

**Byte:** conjunto de 8 bits.

Exemplo:

```text
01000001
```

Esse conjunto possui 8 bits, portanto representa um byte.

### 6.2 Sistema Binário

O sistema binário utiliza apenas dois algarismos: 0 e 1.

Diferentemente do sistema decimal, que utiliza dez algarismos (0 até 9), o sistema binário utiliza potências de 2.

Exemplo:

```text
Decimal: 13

Binário: 1101
```

A conversão pode ser demonstrada assim:

\[
1101_2 = 1(8) + 1(4) + 0(2) + 1(1)
\]

\[
1101_2 = 13_{10}
\]

### 6.3 Representação de Caracteres

Os computadores também precisam representar letras, números e símbolos.

Para isso, utilizam padrões de codificação de caracteres.

Dois exemplos importantes são:

- **ASCII:** padrão de codificação que representa caracteres utilizando valores numéricos.
- **Unicode:** padrão que permite representar caracteres de praticamente todos os sistemas de escrita.

Exemplo:

A letra `A` possui o valor decimal 65 na tabela ASCII.

Sua representação binária em ASCII é:

```text
01000001
```

### 6.4 Representação de Números

Os computadores precisam representar diferentes tipos de números.

**Números inteiros:**

Exemplo:

```text
10
25
-15
100
```

**Números reais:**

Exemplo:

```text
3.14
10.5
-2.75
```

Em linguagens como C++, existem tipos específicos para representar esses valores:

```cpp
int idade = 20;

float altura = 1.75f;

double pi = 3.1415926535;
```

### 6.5 Representação de Imagens, Áudio e Vídeo

Além de textos e números, os computadores também armazenam conteúdos multimídia.

- **Imagens:** representadas por pixels e valores de cores.
- **Áudio:** representado por amostras digitais de sinais sonoros.
- **Vídeo:** representado por uma sequência de quadros (frames), geralmente acompanhada de áudio.

Todos esses dados são armazenados internamente utilizando bits.

---

## 7. Linguagem de Programação

**O que é uma Linguagem de Programação?**

Uma linguagem de programação é um conjunto de regras sintáticas e semânticas que permite escrever instruções para que um computador execute determinadas tarefas.

Por meio dessas linguagens, os desenvolvedores conseguem criar programas, aplicativos, jogos, sistemas operacionais e diversos outros softwares.

**Tipos de Linguagens de Programação**

### 7.1 Linguagens de Baixo Nível

São linguagens que possuem maior proximidade com a arquitetura do computador.

Exemplos:

- Linguagem de máquina.
- Assembly.

A linguagem de máquina utiliza diretamente instruções codificadas em bits.

Assembly utiliza instruções simbólicas que representam operações de processador.

### 7.2 Linguagens de Alto Nível

São linguagens que possuem estruturas mais próximas da forma como os seres humanos escrevem e organizam instruções.

Exemplos:

- C.
- C++.
- Java.
- Python.
- JavaScript.
- C#.

Essas linguagens facilitam o desenvolvimento e a manutenção de programas.

**Exemplo de Linguagem de Programação: C++**

```cpp
#include <iostream>

int main() {

 int numero1 = 10;
 int numero2 = 20;

 int resultado = numero1 + numero2;

 std::cout << "Resultado: " << resultado << std::endl;

 return 0;
}
```

**Resultado**

```text
Resultado: 30
```

Nesse exemplo:

- `#include <iostream>` permite utilizar recursos de entrada e saída.
- `int main()` define a função principal.
- `int` declara variáveis do tipo inteiro.
- `resultado` armazena o resultado da soma.
- `std::cout` apresenta informações na tela.
- `return 0` indica o encerramento normal do programa.

---

## 8. Como todos esses conceitos se relacionam?

Para compreender melhor o funcionamento de um computador, podemos observar como os conceitos estudados trabalham juntos.

Imagine que você deseja executar um programa desenvolvido em C++.

O processo acontece da seguinte maneira:

1. O programador escreve o código-fonte utilizando uma linguagem de programação.
2. Um compilador traduz o código para uma representação executável.
3. O sistema operacional carrega o programa na memória RAM.
4. O processador executa as instruções do programa.
5. Os dados são manipulados internamente utilizando representações binárias.
6. O resultado é apresentado ao usuário por meio de dispositivos de saída.
