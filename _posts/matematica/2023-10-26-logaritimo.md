---
layout: post
title: "Logaritimo"
author: Rebecca
permalink: /matematica/logaritimo
---

Logaritmo de um número é o expoente a que outro valor fixo, a base, deve ser elevado para produzir este número. Por exemplo, o logaritmo de 1 000 na base 10 é 3 porque 10 elevado ao cubo é 1 000 (1 000 = 10 × 10 × 10 = 10³). De maneira geral, para quaisquer dois números reais b e x, onde b é positivo e b ≠ 1.

$$ y = b^x \Leftrightarrow x=\log_b(y) $$

onde:
- $b$ é a base do logaritimo;
- $y$ é o logaritimando;
- $x$ é o proprio logartimo;
- Sendo $log_b(y)$ pronunciado como "o logaritmo de $y$ na base $b$".

Desta forma, o logaritmo é a uma operação na qual queremos descobrir o expoente que uma dada base deve ter para resultar em uma certa potência.

Por esse motivo, para fazer operações com logaritmos é necessário conhecer as propriedades da potenciação.

## Definição
A ideia dos logaritmos é reverter a operação de exponenciação, isto é, elevar um número a uma potência. A título de exemplo, a potência de três (ou o cubo) de 2 é 8, porque 8 é o produto dos três fatores de 2:

$$ 2^3 = 2 \times 2 \times 2 = 8 $$

Disso resulta que o logaritmo de 8 na base 2 é 3, ou seja: $log_2(8) = 3$

Quando a base de um logaritmo for omitida, significa que seu valor é igual a 10. Este tipo de logaritmo é chamado de logaritmo decimal.

### Exemplo
1. $log_2(16) = 4$ visto que $2^4 = 2 \times 2 \times 2 \times 2 = 16$ 

2. $log_3(81) = x \Leftrightarrow 3^x = 81$
Podemos fatorar o número 81:

<code>81 | 3 <br>
27 | 3 <br>
9  | 3 <br>
3  | 3 <br>
1 <br> </code>

$\therefore 3^4$ Logo, x = 4

3. Logaritimos tambem podem ser negativos:

$$log_2(\frac{1}{2}) = -1$$

por que:

$$2^{-1} = \frac{1}{2^1} = \frac{1}{2}$$

## Propriedades
- O logaritmo de qualquer base, cujo logaritmando seja igual a 1, o resultado será igual a 0, ou seja, $log_a(1) = 0$. Por exemplo, $log_9(1) = 0$, pois $9^0 = 1$.
- Quando o logaritmando é igual a base, o logaritmo será igual a 1, assim, $log_a(a) = 1$. Por exemplo, $log_5(5) = 1$, pois $5^1= 5$
- Quando o logaritmo de a na base a possui uma potência m, ele será igual ao expoente m, ou seja $log_a(a^m) = m,$ pois usando a definição $a^m = a^m$. Por exemplo, $log_3(3^5) = 5$.
- Quando dois logaritmos com a mesma base são iguais, os logaritmandos também serão iguais, ou seja, $log_a(b) = log_a(c) \Leftrightarrow b = c$.
- A potência de base a e expoente $log_a(b)$ será igual a b, ou seja $a^{log_a(b)} = b$.

### Produto
O logaritmo de um produto é a soma dos logaritmos dos números a serem multiplicados

$$ \log_b(x y) = \log_b (x) + \log_b (y)$$

ou seja

$$ \log_3 (243) = \log_3(9 \cdot 27) = \log_3 (9) + \log_3 (27) =  2 + 3 = 5 $$

### Quociente
O logaritmo da razão é a diferença dos logaritmos

$$\log_b(\frac{x}{y}) = \log_b(x) - \log_b(y)$$

ou seja

$$ \log_2 (16) = \log_2(\frac{64}{4}) = \log_2 (64) - \log_2 (4) = 6 - 2 = 4 $$

### Potência
O logaritmo da _p_-ésima potência de um número é _p_ vezes o logaritmo do número em questão

$$ \log_b(x^p) = p \log_b (x) $$

ou seja

$$ \log_2 (64) = \log_2 (2^6) = 6 \log_2 (2) = 6 $$

### Mudança de base
Podemos mudar a base de um logaritmo usando a seguinte relação:

$$ log_b(c) = \frac{log_a(c)}{log_a(b)} $$ 

Dado um número x e seu logaritmo $log_b(x)$, a base desconhecida b é dada por:

$$ b = x^\frac{1}{\log_b(x)} $$
