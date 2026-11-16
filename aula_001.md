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

Estuda formas de armazenar, organizar, consultar e gerenciar informações.

### 8.5 Redes de Computadores

Estuda como computadores e outros dispositivos se comunicam e compartilham informações.

### 8.6 Engenharia de Software

Estuda métodos, processos e ferramentas utilizados para desenvolver softwares de maneira organizada e confiável.

### 8.7 Computação Gráfica

Estuda técnicas para criar e manipular imagens, animações e ambientes tridimensionais.

## 9. Por que estudar Ciência da Computação?

Estudar Ciência da Computação permite compreender os fundamentos da tecnologia e desenvolver habilidades para resolver problemas.

Entre os principais benefícios estão:

- Desenvolver raciocínio lógico.
- Aprender a resolver problemas complexos.
- Compreender o funcionamento dos computadores.
- Criar programas e sistemas.
- Desenvolver pensamento computacional.
- Conhecer diferentes áreas da tecnologia.

## 10. Resumo da Aula

Nesta primeira aula, aprendemos:

1. O que é Ciência da Computação.
2. A história e a evolução da computação.
3. O que é um computador.
4. A diferença entre hardware e software.
5. O conceito de programação.
6. O que são algoritmos.
7. O que são linguagens de programação.
8. As principais áreas da Ciência da Computação.
9. A importância de estudar computação.

---

## 11. Exercícios de Fixação

**1. O que é Ciência da Computação?**

**2. Qual é a diferença entre hardware e software?**

**3. O que é um algoritmo?**

**4. Qual é a função do processador (CPU)?**

**5. O que é programação?**

**6. Quem é frequentemente reconhecida como a primeira programadora da história?**

**7. Cite cinco linguagens de programação?**

**8. Quais são as quatro etapas básicas do funcionamento de um computador?**

**9. O que é inteligência artificial?**

**10. Qual é a importância da Ciência da Computação para a sociedade?**

---

## 12. Próxima Aula

**Aula 2 - Fundamentos da Computação**

Conteúdos que serão estudados:

- Sistemas de numeração.
- Sistema binário.
- Sistema decimal.
- Sistema hexadecimal.
- Conversão entre sistemas numéricos.
- Bits e Bytes.
- Representação de dados nos computadores.
- Código ASCII e Unicode.

---

*Fim da Aula 1 - Introdução à Ciência da Computação.*
