# Ciência da Computação — Aula 2

## Fundamentos da Computação

## 1. Introdução aos Fundamentos da Computação

Os fundamentos da computação são os conceitos básicos que explicam como os computadores representam, armazenam, processam e transmitem informações.

Para compreender como um computador funciona internamente, precisamos conhecer conceitos como:

- Sistemas de numeração.
- Sistema binário.
- Sistema decimal.
- Sistema octal.
- Sistema hexadecimal.
- Conversão entre sistemas numéricos.
- Bits e Bytes.
- Representação de dados.
- Código ASCII e Unicode.

Esses conceitos são fundamentais para áreas como programação, arquitetura de computadores, redes, sistemas operacionais e segurança da informação.

---

## 2. Sistemas de Numeração

Um **sistema de numeração** é um conjunto de símbolos e regras utilizados para representar números.

Existem diferentes sistemas de numeração, cada um utilizando uma determinada quantidade de símbolos.

Os principais sistemas utilizados na computação são:

| Sistema | Base | Símbolos utilizados |
|---|---:|---|
| Decimal | 10 | 0 até 9 |
| Binário | 2 | 0 e 1 |
| Octal | 8 | 0 até 7 |
| Hexadecimal | 16 | 0 até 9 e A até F |

O número da base representa a quantidade de símbolos disponíveis em determinado sistema.

### 2.1 Sistema Decimal

O sistema decimal é o sistema de numeração utilizado no nosso cotidiano.

Ele possui base 10, utilizando dez símbolos:

`0, 1, 2, 3, 4, 5, 6, 7, 8, 9`

Cada posição de um número representa uma potência de 10.

**Exemplo:**

Número: `352`

Podemos decompor esse número da seguinte maneira:

```text
352 = 3 × 100 + 5 × 10 + 2 × 1

352 = 300 + 50 + 2
```

Utilizando potências:

```text
352 = 3 × 10² + 5 × 10¹ + 2 × 10⁰
```

### 2.2 Sistema Binário

O sistema binário é um sistema de numeração de base 2.

Ele utiliza apenas dois símbolos:

- `0`
- `1`

Os computadores utilizam o sistema binário para representar e processar informações por meio de estados físicos de circuitos eletrônicos.

Cada posição de um número binário representa uma potência de 2.

**Exemplo:**

Número binário: `1011`

Decomposição:

```text
1011 = 1 × 2³ + 0 × 2² + 1 × 2¹ + 1 × 2⁰
```

Calculando:

```text
1011 = 8 + 0 + 2 + 1

1011 = 11
```

Portanto:

```text
1011₂ = 11₁₀
```

### 2.3 Sistema Octal

O sistema octal possui base 8 e utiliza os seguintes símbolos:

`0, 1, 2, 3, 4, 5, 6, 7`

Cada posição representa uma potência de 8.

**Exemplo:**

Número: `157`

```text
157 = 1 × 8² + 5 × 8¹ + 7 × 8⁰

157 = 64 + 40 + 7

157 = 111
```

Portanto:

```text
157₈ = 111₁₀
```

O sistema octal é utilizado em algumas áreas da computação, especialmente em permissões de arquivos em sistemas Unix e Linux.

### 2.4 Sistema Hexadecimal

O sistema hexadecimal possui base 16.

Ele utiliza dez números e seis letras:

| Decimal | Hexadecimal |
|---:|---|
| 0 | 0 |
| 1 | 1 |
| 2 | 2 |
| 3 | 3 |
| 4 | 4 |
| 5 | 5 |
| 6 | 6 |
| 7 | 7 |
| 8 | 8 |
| 9 | 9 |
| 10 | A |
| 11 | B |
| 12 | C |
| 13 | D |
| 14 | E |
| 15 | F |

Cada posição representa uma potência de 16.

**Exemplo:**

Número hexadecimal: `2A`

```text
2A = 2 × 16¹ + 10 × 16⁰

2A = 32 + 10

2A = 42
```

Portanto:

```text
2A₁₆ = 42₁₀
```

O sistema hexadecimal é muito utilizado na computação porque permite representar números binários de maneira mais compacta.

**Exemplos de aplicações:**

- Endereços de memória.
- Códigos de cores HTML e CSS.
- Depuração de programas.
- Representação de dados binários.

---

## 3. Conversão entre Sistemas Numéricos

A conversão entre sistemas numéricos consiste em transformar um número de uma base para outra.

Essa habilidade é importante para compreender como os computadores representam valores internamente.

### 3.1 Conversão de Binário para Decimal

Para converter um número binário em decimal, devemos multiplicar cada dígito pela potência de 2 correspondente à sua posição.

**Exemplo:**

Converter `1101₂` para decimal.

```text
1101₂

= 1 × 2³
+ 1 × 2²
+ 0 × 2¹
+ 1 × 2⁰

= 8 + 4 + 0 + 1

= 13
```

Resultado:

```text
1101₂ = 13₁₀
```

### 3.2 Conversão de Decimal para Binário

Para converter um número decimal em binário, utilizamos divisões sucessivas por 2.

Devemos dividir o número por 2 e guardar os restos até que o quociente seja zero.

Depois, lemos os restos de baixo para cima.

**Exemplo:**

Converter `13₁₀` para binário.

```text
13 ÷ 2 = 6, resto 1
 6 ÷ 2 = 3, resto 0
 3 ÷ 2 = 1, resto 1
 1 ÷ 2 = 0, resto 1
```

Lendo os restos de baixo para cima:

```text
1101
```

Resultado:

```text
13₁₀ = 1101₂
```

### 3.3 Conversão de Hexadecimal para Decimal

Para converter hexadecimal em decimal, multiplicamos cada dígito pela potência de 16 correspondente.

**Exemplo:**

Converter `3F₁₆` para decimal.

Sabemos que:

```text
F = 15
```

Então:

```text
3F = 3 × 16¹ + 15 × 16⁰

3F = 48 + 15

3F = 63
```

Resultado:

```text
3F₁₆ = 63₁₀
```

### 3.4 Conversão de Decimal para Hexadecimal

Para converter decimal em hexadecimal, realizamos divisões sucessivas por 16.

**Exemplo:**

Converter `42₁₀` para hexadecimal.

```text
42 ÷ 16 = 2, resto 10
 2 ÷ 16 = 0, resto 2
```

O resto 10 corresponde à letra A.

Lendo os restos de baixo para cima:

```text
2A
```

Resultado:

```text
42₁₀ = 2A₁₆
```

### 3.5 Conversão de Binário para Hexadecimal

Para converter binário em hexadecimal, agrupamos os bits de quatro em quatro, começando pela direita.

Cada grupo de quatro bits corresponde a um dígito hexadecimal.

**Exemplo:**

Converter `10101111₂` para hexadecimal.

```text
1010 1111
```

Consultando a correspondência:

```text
1010 = A
1111 = F
```

Resultado:

```text
10101111₂ = AF₁₆
```

### 3.6 Conversão de Hexadecimal para Binário

Cada dígito hexadecimal pode ser representado por quatro bits.

**Exemplo:**

Converter `2F₁₆` para binário.

```text
2 = 0010
F = 1111
```

Resultado:

```text
2F₁₆ = 00101111₂
```

---

## 4. Bits e Bytes

Os computadores trabalham com informações representadas em formato binário.

Para compreender como essas informações são armazenadas, precisamos conhecer os conceitos de bit e byte.

### 4.1 O que é um Bit?

Um **bit** (Binary Digit) é a menor unidade básica de informação utilizada na computação.

Um bit pode assumir apenas dois valores:

- `0`
- `1`

Esses valores representam estados binários utilizados pelos circuitos digitais.

### 4.2 O que é um Byte?

Um **byte** é um conjunto de 8 bits.

Exemplo:

```text
01000001
```

Esse conjunto possui oito bits e corresponde a um byte.

### 4.3 Unidades de Informação

As informações digitais podem ser medidas utilizando diferentes unidades.

| Unidade | Equivalência |
|---|---|
| Bit (b) | Um dígito binário |
| Byte (B) | 8 bits |
| Kilobyte (KB) | 1.000 bytes |
| Megabyte (MB) | 1.000 KB |
| Gigabyte (GB) | 1.000 MB |
| Terabyte (TB) | 1.000 GB |
| Petabyte (PB) | 1.000 TB |

**Observação:** na convenção decimal utilizada para armazenamento, 1 KB corresponde a 1.000 bytes. Na convenção binária, 1 KiB corresponde a 1.024 bytes.

### 4.4 Diferença entre Bit e Byte

É importante não confundir essas duas unidades.

- **Bit (b):** representa um único dígito binário.
- **Byte (B):** representa um conjunto de oito bits.

Exemplos:

```text
1 bit = 0 ou 1

1 byte = 01000001
```

A diferença entre letras maiúsculas e minúsculas também é importante:

- `b` representa bit.
- `B` representa byte.

---

## 5. Representação de Dados nos Computadores

Os computadores precisam representar diferentes tipos de informações utilizando o sistema binário.

Entre essas informações estão:

- Números.
- Textos.
- Imagens.
- Áudios.
- Vídeos.

Tudo isso é armazenado e processado utilizando sequências de bits.

### 5.1 Representação de Números

Os computadores utilizam representações binárias para armazenar números inteiros e números com casas decimais.

Exemplo:

```text
Decimal: 10
Binário: 1010
```

### 5.2 Representação de Textos

Os textos são representados por códigos numéricos associados a caracteres.

Por exemplo, a letra `A` possui o código decimal 65 na tabela ASCII.

Sua representação binária em um byte é:

```text
01000001
```

### 5.3 Representação de Imagens

As imagens digitais são formadas por pequenos elementos chamados pixels.

Cada pixel possui informações que determinam sua cor.

Em imagens RGB, as cores são representadas pela combinação de três componentes:

- Vermelho (Red).
- Verde (Green).
- Azul (Blue).

Cada componente normalmente utiliza 8 bits.

Exemplo:

```text
RGB(255, 0, 0)
```

Representa a cor vermelha.

### 5.4 Representação de Áudios

Os computadores representam áudios por meio de dados digitais.

Um áudio digital é produzido a partir de amostras de um sinal sonoro.

Dois conceitos importantes são:

- **Taxa de amostragem:** quantidade de amostras capturadas por segundo.
- **Profundidade de bits:** quantidade de bits utilizada para representar cada amostra.

### 5.5 Representação de Vídeos

Um vídeo digital é formado por uma sequência de imagens exibidas em determinada velocidade.

Além das imagens, os arquivos de vídeo podem armazenar informações de áudio, legendas e outros dados.

A quantidade de quadros por segundo é chamada de FPS (Frames Per Second).

---

## 6. Código ASCII

ASCII significa **American Standard Code for Information Interchange**.

É um padrão de codificação utilizado para representar caracteres por meio de valores numéricos.

O ASCII tradicional utiliza 7 bits, permitindo representar 128 códigos diferentes.

Esses códigos incluem:

- Letras maiúsculas.
- Letras minúsculas.
- Números.
- Símbolos.
- Caracteres de controle.

### 6.1 Exemplos de códigos ASCII

| Caractere | Decimal | Binário |
|---|---:|---|
| A | 65 | 01000001 |
| B | 66 | 01000010 |
| C | 67 | 01000011 |
| a | 97 | 01100001 |
| b | 98 | 01100010 |
| 0 | 48 | 00110000 |
| 1 | 49 | 00110001 |
| Espaço | 32 | 00100000 |

### 6.2 Exemplo prático

A palavra `ABC` pode ser representada utilizando códigos ASCII:

```text
A = 65
B = 66
C = 67
```

Em binário:

```text
A = 01000001
B = 01000010
C = 01000011
```

Portanto:

```text
ABC = 01000001 01000010 01000011
```

---

## 7. Unicode

O **Unicode** é um padrão desenvolvido para permitir a representação de caracteres utilizados em diferentes idiomas e sistemas de escrita.

Enquanto o ASCII tradicional representa 128 códigos, o Unicode possui um repertório muito maior de caracteres.

Ele permite representar:

- Letras do alfabeto latino.
- Caracteres acentuados.
- Caracteres chineses.
- Caracteres japoneses.
- Caracteres árabes.
- Símbolos matemáticos.
- Emojis.

### 7.1 UTF-8

UTF-8 é uma das formas de codificação utilizadas para representar caracteres Unicode.

Ele utiliza de 1 a 4 bytes por caractere.

Uma de suas principais vantagens é a compatibilidade com o ASCII tradicional.

### 7.2 Exemplo

A letra `A` possui o mesmo valor em ASCII e UTF-8:

```text
A = 65
```

Em hexadecimal:

```text
41
```

Já caracteres acentuados, como `á`, precisam de mais de um byte em UTF-8.

**Exemplo:**

```text
á = C3 A1
```

### 7.3 Diferença entre ASCII e Unicode

| ASCII | Unicode |
|---|---|
| Padrão de codificação tradicional | Padrão universal de caracteres |
| ASCII tradicional possui 128 códigos | Possui um repertório muito maior |
| Limitado principalmente a caracteres básicos | Suporta diversos idiomas e símbolos |
| Utiliza 7 bits | Utiliza diferentes formas de codificação |

---

## 8. Importância dos Fundamentos da Computação

Compreender os fundamentos da computação é essencial para qualquer pessoa que deseja trabalhar com tecnologia.

Esses conhecimentos ajudam a entender:

- Como os computadores armazenam informações.
- Como os processadores trabalham com dados.
- Como os programas representam números e caracteres.
- Como funcionam os sistemas digitais.
- Como os dados são transmitidos pelas redes.
- Como os arquivos são armazenados.

Esses conceitos também são importantes para estudar arquitetura de computadores, programação de baixo nível, sistemas operacionais e engenharia de software.

---

## 9. Resumo da Aula

Nesta aula, estudamos os principais fundamentos da computação:

1. Conceito de sistemas de numeração.
2. Sistema decimal.
3. Sistema binário.
4. Sistema octal.
5. Sistema hexadecimal.
6. Conversão entre sistemas numéricos.
7. Conceitos de bits e bytes.
8. Unidades de armazenamento.
9. Representação de dados nos computadores.
10. Código ASCII.
11. Unicode e UTF-8.

---

## 10. Exercícios de Fixação

### Questões Teóricas

**1.** O que é um sistema de numeração?

**2.** Qual é a base do sistema binário?

**3.** Quais símbolos são utilizados no sistema hexadecimal?

**4.** Qual é a diferença entre bit e byte?

**5.** Quantos bits existem em um byte?

**6.** O que significa ASCII?

**7.** Qual é a principal finalidade do Unicode?

**8.** O que é UTF-8?

**9.** Como os computadores representam imagens digitalmente?

**10.** Por que o sistema binário é utilizado nos computadores?

### Exercícios de Conversão

**11.** Converta o número binário `1010` para decimal.

**12.** Converta o número decimal `25` para binário.

**13.** Converta o número hexadecimal `2F` para decimal.

**14.** Converta o número decimal `64` para hexadecimal.

**15.** Converta o número binário `11110000` para hexadecimal.

**16.** Converta o número hexadecimal `A5` para binário.

**17.** Converta o número octal `25` para decimal.

**18.** Converta o número decimal `100` para binário.

---

## 11. Próxima Aula

### Aula 3 — Lógica de Programação e Algoritmos

Conteúdos que serão estudados:

- Introdução à lógica de programação.
- O que é raciocínio lógico?
- O que é pensamento computacional?
- Algoritmos e suas características.
- Pseudocódigo.
- Fluxogramas.
- Variáveis e constantes.
- Tipos de dados.
- Operadores.
- Entrada e saída de dados.
- Resolução de problemas utilizando algoritmos.

---

*Fim da Aula 2 — Fundamentos da Computação.*
