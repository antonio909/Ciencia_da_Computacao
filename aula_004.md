
# Ciência da Computação — Aula 4
## Introdução à Programação

## 1. Introdução à Programação

A **programação** é o processo de desenvolver instruções que um computador pode executar para realizar determinadas tarefas.

Essas instruções são escritas utilizando linguagens de programação, que permitem aos desenvolvedores criar softwares, aplicativos, jogos, sistemas e diversas outras soluções tecnológicas.

A programação está presente em praticamente todos os setores da sociedade moderna.

**Exemplos de aplicações:**

- Desenvolvimento de sites.
- Aplicativos para celulares.
- Jogos digitais.
- Sistemas bancários.
- Inteligência artificial.
- Sistemas operacionais.
- Automação industrial.
- Sistemas de gerenciamento de dados.

Programar significa transformar um problema em uma sequência de instruções que um computador consegue executar.

### 1.1 Como funciona a programação?

De maneira simplificada, o processo de programação envolve algumas etapas:

1. Identificar um problema.
2. Analisar o que precisa ser resolvido.
3. Desenvolver um algoritmo.
4. Escrever o código-fonte.
5. Compilar ou interpretar o programa, conforme a linguagem.
6. Executar o programa.
7. Testar e corrigir possíveis erros.

**Exemplo:**

Imagine que precisamos desenvolver uma calculadora simples.

O programa deverá:

- Receber dois números.
- Realizar uma operação matemática.
- Apresentar o resultado.

Podemos implementar essa solução utilizando uma linguagem como C++.

---

## 2. O que são Linguagens de Programação?

Uma **linguagem de programação** é um conjunto de regras, símbolos e palavras-chave utilizados para escrever instruções que podem ser processadas por um computador.

Cada linguagem possui sua própria sintaxe e características.

As linguagens permitem que os programadores expressem algoritmos de maneira estruturada.

### 2.1 Principais Linguagens de Programação

| Linguagem | Principais aplicações |
|---|---|
| C | Sistemas operacionais e programação de baixo nível |
| C++ | Jogos, sistemas e aplicações de alto desempenho |
| Python | Inteligência artificial, automação e ciência de dados |
| Java | Sistemas empresariais e aplicações multiplataforma |
| JavaScript | Desenvolvimento web |
| C# | Aplicações desktop, web e jogos |
| PHP | Desenvolvimento backend |
| Rust | Sistemas e aplicações de alto desempenho |
| Go | Sistemas distribuídos e serviços backend |
| Kotlin | Aplicações Android e desenvolvimento multiplataforma |

### 2.2 Por que existem diferentes linguagens?

Cada linguagem foi desenvolvida com características e objetivos específicos.

Algumas oferecem maior controle sobre o hardware, enquanto outras priorizam produtividade, simplicidade ou recursos especializados.

Por exemplo:

- C é muito utilizada em sistemas que exigem controle de baixo nível.
- C++ permite desenvolver aplicações de alto desempenho.
- Python possui sintaxe relativamente simples e é bastante utilizada em inteligência artificial.
- JavaScript é fundamental para o desenvolvimento web.
- Rust oferece recursos importantes para segurança de memória.

Não existe uma única linguagem ideal para todos os problemas.

---

## 3. Linguagens de Baixo e Alto Nível

As linguagens de programação podem ser classificadas de acordo com seu nível de abstração em relação ao hardware.

As duas categorias principais são:

- Linguagens de baixo nível.
- Linguagens de alto nível.

### 3.1 Linguagens de Baixo Nível

As linguagens de baixo nível possuem uma relação mais próxima com a arquitetura do computador.

Elas oferecem maior controle sobre os recursos do hardware.

As principais características são:

- Maior proximidade com o funcionamento do processador.
- Maior controle sobre a memória.
- Menor nível de abstração.
- Maior dependência da arquitetura utilizada.

**Exemplos:**

- Linguagem de máquina.
- Assembly.

### 3.2 Linguagem de Máquina

A linguagem de máquina é formada por instruções representadas em formato binário, que são diretamente executadas pelo processador.

Exemplo ilustrativo:

```text
10110000 01100001
```

O significado dessas instruções depende da arquitetura do processador.

### 3.3 Linguagem Assembly

Assembly utiliza instruções simbólicas para representar operações realizadas pelo processador.

Exemplo ilustrativo:

```asm
MOV AX, 10
ADD AX, 5
```

Nesse exemplo, as instruções representam operações de movimentação e adição de valores.

Assembly facilita a leitura e a escrita de instruções de máquina, mas ainda exige conhecimento da arquitetura do processador.

### 3.4 Linguagens de Alto Nível

As linguagens de alto nível possuem maior abstração em relação ao hardware.

Elas permitem escrever programas utilizando estruturas mais próximas da linguagem humana e da lógica matemática.

Características:

- Sintaxe mais compreensível.
- Maior produtividade.
- Menor dependência direta do hardware.
- Facilidade de manutenção.
- Recursos que simplificam o desenvolvimento.

**Exemplos:**

- C.
- C++.
- Python.
- Java.
- JavaScript.
- C#.

**Exemplo em C++:**

```cpp
#include <iostream>

int main() {

    int numero = 10;

    std::cout << numero;

    return 0;
}
```

O código é muito mais compreensível para um programador do que sua representação em instruções de máquina.

### 3.5 Diferença entre Baixo e Alto Nível

| Baixo Nível | Alto Nível |
|---|---|
| Mais próximo do hardware | Mais próximo da linguagem humana |
| Maior controle sobre recursos físicos | Maior nível de abstração |
| Sintaxe geralmente mais complexa | Sintaxe geralmente mais simples |
| Maior dependência da arquitetura | Geralmente maior portabilidade |
| Exemplo: Assembly | Exemplo: Python e C++ |

---

## 4. Linguagens Compiladas e Interpretadas

As linguagens de programação também podem ser estudadas de acordo com a maneira como seus programas são traduzidos e executados.

Duas categorias frequentemente utilizadas para explicar esse processo são:

- Linguagens compiladas.
- Linguagens interpretadas.

É importante entender que essa classificação é uma simplificação didática. Algumas linguagens utilizam combinações de compilação, interpretação e execução por máquinas virtuais.

### 4.1 Linguagens Compiladas

Uma linguagem compilada utiliza um processo de tradução do código-fonte para uma representação executável ou intermediária antes da execução.

Um compilador analisa o código e realiza essa tradução.

**Exemplos comuns:**

- C.
- C++.
- Rust.

**Características:**

- O código passa por um processo de compilação.
- Erros de compilação podem ser identificados antes da execução.
- Pode produzir arquivos executáveis.
- Permite diversas otimizações durante a compilação.

### 4.2 Linguagens Interpretadas

Nas linguagens interpretadas, um interpretador participa diretamente do processo de execução do programa.

O interpretador analisa e executa as instruções de acordo com o funcionamento da implementação da linguagem.

**Exemplos frequentemente associados a esse modelo:**

- Python.
- JavaScript.
- Ruby.

**Características:**

- Utilizam um ambiente de execução.
- Podem executar instruções sem gerar previamente um executável nativo independente.
- Facilitam determinados fluxos de desenvolvimento.
- O comportamento depende da implementação utilizada.

### 4.3 Comparação

| Linguagens Compiladas | Linguagens Interpretadas |
|---|---|
| Utilizam compilação | Utilizam interpretação durante a execução |
| Podem gerar executáveis nativos | Geralmente dependem de um ambiente de execução |
| Permitem otimizações durante a compilação | Podem realizar otimizações durante a execução |
| Exemplo: C++ | Exemplo: Python |

### 4.4 Linguagens com Execução Híbrida

Algumas linguagens utilizam um modelo híbrido.

**Exemplo: Java**

O código Java normalmente passa pelas seguintes etapas:

1. O programador escreve o código-fonte.
2. O compilador Java transforma o código em bytecode.
3. A Java Virtual Machine (JVM) executa o bytecode.
4. A JVM pode utilizar interpretação e compilação JIT para executar e otimizar o programa.

Esse modelo combina diferentes técnicas de execução.

---

## 5. O que é um Compilador?

Um **compilador** é um programa responsável por traduzir código escrito em uma linguagem de programação para outra representação.

No caso de C++, o compilador normalmente transforma o código-fonte em código de máquina, por meio de etapas intermediárias.

Entre suas principais responsabilidades estão:

- Analisar a sintaxe.
- Verificar regras semânticas.
- Identificar determinados erros.
- Otimizar o código.
- Gerar código de máquina ou outro formato de saída.

### 5.1 Exemplos de Compiladores

| Compilador | Linguagens |
|---|---|
| GCC | C e C++ |
| Clang | C, C++ e Objective-C |
| MSVC | C e C++ |
| Rustc | Rust |
| G++ | C++ |

### 5.2 Exemplo de Compilação em C++

Considere o seguinte código:

```cpp
#include <iostream>

int main() {

    std::cout << "Ola, mundo!";

    return 0;
}
```

Podemos utilizar o compilador G++ para gerar um executável.

Comando:

```bash
g++ main.cpp -o programa
```

Nesse comando:

- `g++`: chama o compilador C++.
- `main.cpp`: arquivo com o código-fonte.
- `-o`: define o nome do arquivo de saída.
- `programa`: nome do executável gerado.

Para executar no Linux:

```bash
./programa
```

No Windows, normalmente:

```powershell
.\programa.exe
```

---

## 6. O que é um Interpretador?

Um **interpretador** é um programa responsável por executar instruções de uma linguagem de programação por meio de um ambiente de execução.

Ele pode analisar o código, executar instruções ou trabalhar com alguma representação intermediária.

### 6.1 Exemplos de Interpretadores e Ambientes de Execução

| Tecnologia | Linguagem |
|---|---|
| CPython | Python |
| Node.js | JavaScript |
| Ruby MRI | Ruby |
| PHP Interpreter | PHP |

### 6.2 Exemplo em Python

Considere o seguinte código:

```python
print("Ola, mundo!")
```

Podemos executar o programa utilizando o interpretador Python:

```bash
python main.py
```

Resultado:

```text
Ola, mundo!
```

O ambiente Python interpreta e executa o programa.

---

## 7. O que é Código-Fonte?

O **código-fonte** é o conjunto de instruções escritas pelo programador utilizando uma linguagem de programação.

Ele representa a implementação de um algoritmo em uma linguagem específica.

O código-fonte pode ser criado em editores de texto ou ambientes de desenvolvimento.

**Exemplo em C++:**

```cpp
#include <iostream>

int main() {

    std::cout << "Meu primeiro programa!";

    return 0;
}
```

Nesse exemplo, todo o conteúdo escrito em C++ representa o código-fonte.

### 7.1 Extensões de Arquivos

Cada linguagem utiliza determinadas extensões para identificar seus arquivos.

| Linguagem | Extensão |
|---|---|
| C | `.c` |
| C++ | `.cpp` |
| Python | `.py` |
| Java | `.java` |
| JavaScript | `.js` |
| C# | `.cs` |
| PHP | `.php` |
| Rust | `.rs` |
| Go | `.go` |

---

## 8. O que é Código de Máquina?

O **código de máquina** é uma representação de instruções em um formato que o processador consegue executar diretamente.

Ele é específico da arquitetura do processador.

Diferentemente do código-fonte, o código de máquina não utiliza palavras e estruturas desenvolvidas para facilitar a leitura humana.

Suas instruções são representadas por padrões binários.

### 8.1 Exemplo Ilustrativo

Uma sequência de bits pode representar uma instrução de máquina:

```text
10110000 01100001
```

Essa sequência é apenas ilustrativa. O significado real depende da arquitetura e do conjunto de instruções do processador.

### 8.2 Diferença entre Código-Fonte e Código de Máquina

| Código-Fonte | Código de Máquina |
|---|---|
| Escrito pelo programador | Gerado por um processo de tradução |
| Utiliza uma linguagem de programação | Utiliza instruções da arquitetura |
| Mais compreensível para humanos | Interpretado diretamente pelo processador |
| Exemplo: C++ | Instruções binárias |

---

## 9. Processo de Compilação

O processo de compilação transforma o código-fonte em uma representação que pode ser executada pelo computador.

No desenvolvimento de programas em C e C++, esse processo normalmente envolve quatro etapas principais:

1. Pré-processamento.
2. Compilação.
3. Montagem.
4. Ligação.

### 9.1 Pré-processamento

O pré-processador analisa diretivas iniciadas pelo símbolo `#`.

Entre suas responsabilidades estão:

- Incluir arquivos de cabeçalho.
- Expandir macros.
- Processar diretivas condicionais.

**Exemplo:**

```cpp
#include <iostream>
#define PI 3.14159
```

Nesse caso:

- `#include` solicita a inclusão de um cabeçalho.
- `#define` define uma macro.

### 9.2 Compilação

Nessa etapa, o compilador analisa o código pré-processado e o transforma em código Assembly ou outra representação intermediária.

Também realiza análises sintáticas e semânticas e pode aplicar otimizações.

### 9.3 Montagem

O montador transforma o código Assembly em código de máquina armazenado em arquivos objeto.

Esses arquivos podem conter instruções e referências que ainda precisam ser resolvidas.

### 9.4 Ligação (Linking)

O linker combina arquivos objeto e bibliotecas necessárias para produzir o executável final.

Ele também resolve referências entre diferentes partes do programa.

### 9.5 Fluxo de Compilação

```text
       Código-fonte
             |
             v
      Pré-processamento
             |
             v
         Compilação
             |
             v
          Assembly
             |
             v
          Montagem
             |
             v
       Arquivo objeto
             |
             v
           Linker
             |
             v
         Executável
             |
             v
          Execução
```

---

## 10. Introdução à Linguagem C++

O **C++** é uma linguagem de programação de propósito geral, desenvolvida por Bjarne Stroustrup como uma extensão da linguagem C.

Sua primeira versão foi desenvolvida no início da década de 1980.

A linguagem combina recursos de programação procedural, orientação a objetos, programação genérica e outros paradigmas.

### 10.1 Principais Características do C++

- Alto desempenho.
- Controle sobre recursos de memória.
- Programação orientada a objetos.
- Programação genérica utilizando templates.
- Suporte à programação procedural.
- Biblioteca padrão abrangente.
- Compatibilidade com diferentes plataformas.
- Utilização em sistemas complexos.

### 10.2 Onde C++ é Utilizado?

O C++ possui aplicações em diversas áreas da tecnologia.

**Desenvolvimento de jogos:**

Utilizado em motores gráficos e jogos que exigem alto desempenho.

**Sistemas operacionais:**

Utilizado no desenvolvimento de componentes de sistemas e softwares de baixo nível.

**Aplicações de alto desempenho:**

Utilizado em sistemas que precisam processar grandes quantidades de informações.

**Computação gráfica:**

Utilizado em motores gráficos, simulações e aplicações tridimensionais.

**Sistemas embarcados:**

Utilizado em dispositivos eletrônicos e equipamentos especializados.

**Aplicações financeiras:**

Utilizado em sistemas que exigem baixa latência e processamento eficiente.

---

## 11. Estrutura Básica de um Programa C++

Todo programa C++ possui uma estrutura que organiza suas instruções.

Observe o exemplo:

```cpp
#include <iostream>

int main() {

    std::cout << "Ola, mundo!";

    return 0;
}
```

Vamos entender cada parte.

### 11.1 Biblioteca iostream

```cpp
#include <iostream>
```

A diretiva `#include` permite incluir um cabeçalho da biblioteca padrão.

O cabeçalho `iostream` fornece recursos para entrada e saída de dados.

Entre eles estão:

- `std::cout`: saída de dados.
- `std::cin`: entrada de dados.
- `std::cerr`: saída de mensagens de erro.

### 11.2 Função main()

```cpp
int main() {

}
```

A função `main()` é o ponto de entrada de um programa C++ executável.

É nela que começa a execução normal do programa.

O tipo `int` indica que a função retorna um número inteiro ao ambiente de execução.

### 11.3 Instrução std::cout

```cpp
std::cout << "Ola, mundo!";
```

O objeto `std::cout` é utilizado para apresentar informações na saída padrão, normalmente o terminal.

O operador `<<` envia informações para a saída.

### 11.4 Instrução return 0

```cpp
return 0;
```

Indica que a função `main()` terminou com um código de retorno igual a zero.

Tradicionalmente, esse valor indica que o programa terminou com sucesso.

### 11.5 Ponto e Vírgula

Em C++, a maioria das instruções simples termina com ponto e vírgula.

Exemplo:

```cpp
int idade = 20;

std::cout << idade;

return 0;
```

Esquecer o ponto e vírgula pode provocar um erro de compilação.

---

## 12. Primeiro Programa em C++

Agora que conhecemos a estrutura básica de um programa, podemos desenvolver nosso primeiro exemplo.

### 12.1 Código Completo

```cpp
#include <iostream>

int main() {

    std::cout << "Ola, mundo!";

    return 0;
}
```

### 12.2 Resultado

```text
Ola, mundo!
```

Esse programa apresenta uma mensagem no terminal.

### 12.3 Exemplo com Múltiplas Linhas

Podemos apresentar diferentes mensagens utilizando `std::cout`.

```cpp
#include <iostream>

int main() {

    std::cout << "Bem-vindo a Ciencia da Computacao!\n";

    std::cout << "Estamos aprendendo C++.\n";

    std::cout << "Este e nosso primeiro programa.";

    return 0;
}
```

Resultado:

```text
Bem-vindo a Ciencia da Computacao!
Estamos aprendendo C++.
Este e nosso primeiro programa.
```

O caractere `\n` representa uma quebra de linha.

---

## 13. Ambientes de Desenvolvimento

Para desenvolver programas, precisamos de ferramentas que permitam escrever, compilar, executar e depurar código.

Essas ferramentas podem ser utilizadas individualmente ou integradas em ambientes de desenvolvimento.

### 13.1 Editor de Código

Um editor de código é um programa utilizado para escrever e editar arquivos de código-fonte.

Exemplos:

- Visual Studio Code.
- Sublime Text.
- Vim.
- Notepad++.

### 13.2 IDE

IDE significa **Integrated Development Environment**, ou Ambiente de Desenvolvimento Integrado.

Uma IDE reúne diferentes ferramentas em uma única aplicação.

Normalmente oferece:

- Editor de código.
- Compilador ou integração com compiladores.
- Depurador.
- Gerenciamento de projetos.
- Ferramentas de execução.

Exemplos:

- Visual Studio.
- CLion.
- Code::Blocks.
- Qt Creator.

### 13.3 Compiladores C++

Alguns compiladores utilizados para desenvolver aplicações em C++ são:

- GCC.
- Clang.
- MSVC.

O compilador transforma o código-fonte em uma representação executável.

---

## 14. Importância de Aprender Programação

Aprender programação permite compreender como os sistemas digitais funcionam e desenvolver soluções para problemas reais.

Entre as principais habilidades desenvolvidas estão:

- Raciocínio lógico.
- Pensamento computacional.
- Resolução de problemas.
- Organização de código.
- Análise de algoritmos.
- Desenvolvimento de software.
- Conhecimento sobre computadores.

A programação também é uma ferramenta importante para áreas como engenharia, ciência de dados, robótica, inteligência artificial e automação.

---

## 15. Resumo da Aula

Nesta aula, estudamos:

1. Conceito de programação.
2. Linguagens de programação.
3. Linguagens de baixo nível.
4. Linguagens de alto nível.
5. Linguagens compiladas.
6. Linguagens interpretadas.
7. Modelos híbridos de execução.
8. Compiladores.
9. Interpretadores.
10. Código-fonte.
11. Código de máquina.
12. Processo de compilação.
13. Introdução à linguagem C++.
14. Estrutura básica de um programa C++.
15. Primeiro programa em C++.
16. Editores de código e IDEs.

---

## 16. Exercícios de Fixação

### Questões Teóricas

**1.** O que é programação?

**2.** O que são linguagens de programação?

**3.** Qual é a diferença entre linguagens de baixo e alto nível?

**4.** O que é linguagem de máquina?

**5.** O que é Assembly?

**6.** Qual é a diferença entre linguagens compiladas e interpretadas?

**7.** O que é um compilador?

**8.** O que é um interpretador?

**9.** O que é código-fonte?

**10.** O que é código de máquina?

**11.** Quais são as principais etapas do processo de compilação em C++?

**12.** Quem desenvolveu a linguagem C++?

**13.** Quais são algumas aplicações da linguagem C++?

**14.** Qual é a finalidade da função `main()`?

**15.** Para que serve a biblioteca `iostream`?

**16.** Qual é a função de `std::cout`?

**17.** Qual é a finalidade da instrução `return 0`?

**18.** Qual é a diferença entre um editor de código e uma IDE?

### Exercícios Práticos

**19.** Crie um programa em C++ que apresente a mensagem `Ola, mundo!`.

**20.** Crie um programa que apresente seu nome, sua idade e sua cidade.

**21.** Crie um programa que apresente três mensagens diferentes, cada uma em uma linha.

**22.** Crie um programa que apresente o resultado da soma de dois números utilizando valores definidos diretamente no código.

**23.** Explique a função de cada instrução utilizada no seu primeiro programa em C++.

---

## 17. Próxima Aula

# Aula 5 — Arquitetura de Computadores

Conteúdos que serão estudados:

- Introdução à arquitetura de computadores.
- Organização de computadores.
- Unidade Central de Processamento (CPU).
- Unidade de Controle (CU).
- Unidade Lógica e Aritmética (ALU).
- Registradores.
- Memória RAM.
- Memória ROM.
- Memória Cache.
- Barramentos.
- Ciclo de instrução.
- Arquitetura Von Neumann.
- Arquitetura Harvard.
- Dispositivos de entrada e saída.

---

*Fim da Aula 4 — Introdução à Programação.*
