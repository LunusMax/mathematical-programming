# Exercício 8 — Verdadeiro ou Falso

Julgue as afirmações abaixo como verdadeiras (V) ou falsas (F).

Caso haja afirmação(ões) falsa(s), apresente o(s) erro(s) e faça a(s) correção(ões).

## (a)

Para um mesmo problema, podem existir mais de uma formulação matemática correta.

**Resposta:**

Verdadeiro.

---

## (b)

Dadas as constantes $`n`$ e $`c_i`$, e as variáveis $`x_i \in \mathbb{R}`$, com $`i = 1,\ldots,n`$, a função

```math
x_1 \sum_{i=1}^{n} c_i x_i
```

é uma função linear.

**Resposta:**

Falso, pois, expandindo a somatória, temos:

```math
x_1 \sum_{i=1}^{n} c_i x_i
=
x_1c_1x_1 + x_1c_2x_2 + \cdots + x_1c_nx_n
```

ou seja,

```math
c_1x_1^2 + c_2x_1x_2 + \cdots + c_nx_1x_n.
```

Portanto, aparecem termos não lineares, como $`x_1^2`$ e $`x_1x_2`$.

Para que a função fosse linear, não poderia haver o fator $`x_1`$ multiplicando a somatória.

---

## (c)

Dadas as constantes $`c_1`$ e $`c_2`$, e a variável $`x_1 \in \mathbb{R}`$,

```math
c_1c_2x_1
```

é uma função linear.

**Resposta:**

Verdadeiro.

---

## (d)

Em um PL (programa linear), podemos restringir uma variável a ser não-negativa.

**Resposta:**

Verdadeiro. Uma variável pode ser restringida por

```math
x \geq 0.
```

---

## (e)

Em um PL, podemos restringir uma variável a ser não-positiva.

**Resposta:**

Verdadeiro.

---

## (f)

PLs na forma padrão só admitem variáveis não-negativas.

**Resposta:**

Verdadeiro.

---

## (g)

Uma variável $`x`$ em um PL pode ser

```math
x \geq -1
```

ou

```math
x \leq 1.
```

**Resposta:**

Verdadeiro.

---

## (h)

Uma variável $`x`$ em um PL pode ser

```math
x \geq -1
```

e

```math
x \leq 1.
```

**Resposta:**

Verdadeiro. Nesse caso,

```math
-1 \leq x \leq 1.
```

---

## (i)

Restrições do tipo $`<`$ e $`>`$ são admitidas em um PL.

**Resposta:**

Falso. Em Programação Linear são utilizadas restrições dos tipos

```math
\leq,\quad \geq,\quad =
```

e não desigualdades estritas.

---

## (j)

Regiões factíveis ilimitadas não admitem solução ótima única.

**Resposta:**

Falso, pois uma região factível ilimitada não significa que a função objetivo seja ilimitada.

Por exemplo:

```math
\min \; x_1 + x_2
```

sujeito a

```math
x_1, x_2 \geq 0.
```

A região factível é ilimitada, mas existe uma solução ótima única em

```math
(x_1,x_2)=(0,0).
```

---

## (k)
Em uma dada iteração do Simplex em Tabelas, se constatarmos que a solução do problema é ilimitada, então pelo menos uma das variáveis não-básicas com custo relativo menor que zero terá sua coluna composta por elementos nulos ou negativos.

**Resposta:**
Verdadeiro.

---

## (l)
Caso o critério de otimalidade do Simplex for alcançado, se obtivermos ao menos uma variável não-básica com custo relativo igual a zero, podemos afirmar que temos múltiplas soluções ótimas.

**Resposta:**
Falso, pois custo relativo igual a zero não garante a existência de múltiplas soluções ótimas.

---

## (m)
Se a região factível possui um vértice, então o problema possui solução ótima.

**Resposta:**
Falso. A existência de um vértice não garante a existência de uma solução ótima, pois a função objetivo pode melhorar indefinidamente em uma região factível ilimitada.

---

## (n)
De um modo geral, um problema artificial possui múltiplas soluções ótimas.

**Resposta:**
Falso. Um problema artificial pode possuir solução ótima única ou múltiplas soluções ótimas; não é possível afirmar, de modo geral, que sempre haverá multiplicidade.

---

## (o)
Se um PL tem infinitas soluções ótimas, então seu problema artificial possui solução diferente de zero.

**Resposta:**
Falso. Se o problema original possui soluções ótimas, então ele é factível. Portanto, no Método das Duas Fases, o valor ótimo do problema artificial deve ser igual a zero.

---

## (p)
Toda solução factível é básica.

**Resposta:**
Falso. Uma solução factível satisfaz todas as restrições do problema, mas não precisa ser uma solução básica. Geometricamente, existem pontos factíveis que não são vértices da região factível.

---

## (q)
Toda solução básica é factível.

**Resposta:**
Falso. Uma solução básica pode possuir alguma variável básica negativa. Ela só será uma solução básica factível se também satisfizer as condições de factibilidade, em particular a não-negatividade das variáveis.

---

## (r)
Se um problema possui solução ótima, então existe um vértice ótimo.

**Resposta:**
Verdadeiro.

---

## (s)
Existe uma regra de pivoteamento tal que o método Simplex é um algoritmo polinomial para resolver PLs.

**Resposta:**
Falso. Não é conhecida uma regra de pivoteamento do Método Simplex que garanta um número polinomial de iterações para todo problema de Programação Linear.

---

## (u)
Se o método Simplex entra num ciclo, então uma solução básica degenerada se repete.

**Resposta:**
Verdadeiro.


## Exercício 9

Por quê uma solução básica factível é candidata a ser a solução ótima de um problema linear?

**Resposta:**

Uma solução básica factível é candidata à solução ótima porque ela corresponde a um vértice da região factível. Em um problema linear, se existir uma solução ótima finita, então existe pelo menos uma solução ótima em um vértice da região factível. Por isso, o Método Simplex busca a solução ótima percorrendo soluções básicas factíveis.