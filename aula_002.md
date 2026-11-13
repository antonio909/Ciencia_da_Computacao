# Ciência da Computação - Aula 2
## Fundamentos da Computação

## 1. Introdução aos Fundamentos da Computação

Os fundamentos da computação são os conceitos básicos que explicam como os computadores representam, armazenam, processam e transmitem informações.

Para compreender como um computador funciona internamente, precisamos conhecer conceitos como:

- Sistemas de numeração.
- Sistema binário.
- Sistema decimal.
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
352 = 3 x 100 + 5 x 10 + 2 x 1

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
