# Exercício 8 — Verdadeiro ou Falso

Julgue as afirmações abaixo como verdadeiras (V) ou falsas (F).  
Caso haja afirmação(ões) falsa(s), apresente o(s) erro(s) e faça a(s) correção(ões).

## (a)
Para um mesmo problema, podem existir mais de uma formulação matemática correta.

**Resposta:**
Verdadeiro.

---

## (b)
Dadas as constantes \(n\) e \(c_i\), e as variáveis \(x_i \in \mathbb{R}\), com \(i = 1,\ldots,n\), a função

\[
x_1 \sum_{i=1}^{n} c_i x_i
\]

é uma função linear.

**Resposta:**
Falso, pois, expandindo a somatória, temos:

\[
x_1 \sum_{i=1}^{n} c_i x_i
=
x_1c_1x_1 + x_1c_2x_2 + \cdots + x_1c_nx_n
\]

ou seja,

\[
c_1x_1^2 + c_2x_1x_2 + \cdots + c_nx_1x_n.
\]

Portanto, aparecem termos não lineares, como \(x_1^2\) e \(x_1x_2\).

Para que a função fosse linear, não poderia haver o fator \(x_1\) multiplicando a somatória.

---

## (c)
Dados as constantes \(c_1\) e \(c_2\), e a variável \(x_1 \in \mathbb{R}\),

\[
c_1 c_2 x_1
\]

é uma função linear.

**Resposta:**
Verdadeiro.

---

## (d)
Em um PL (programa linear), podemos restringir uma variável a ser não-negativa.

**Resposta:**
Verdadeiro. Uma variável pode ser restringida por

\[
x \geq 0.
\]

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
Uma variável \(x\) em um PL pode ser

\[
x \geq -1
\]

ou

\[
x \leq 1.
\]

**Resposta:**
Verdadeiro.

---

## (h)
Uma variável \(x\) em um PL pode ser

\[
x \geq -1
\]

e

\[
x \leq 1.
\]

**Resposta:**
Verdadeiro.

---

## (i)
Restrições do tipo

\[
<
\]

e

\[
>
\]

são admitidas em um PL.

**Resposta:**
Falso. Em Programação Linear são utilizadas restrições dos tipos

\[
\leq,\quad \geq,\quad =
\]

e não desigualdades estritas.


---

## (j)
Regiões factíveis ilimitadas não admitem solução ótima única.

**Resposta:**
Falso, pois uma região factível ilimitada não significa que a função objetivo seja ilimitada.

Por exemplo:

\[
\min x_1+x_2
\]

sujeito a

\[
x_1,x_2 \geq 0.
\]

A região factível é ilimitada, mas existe uma solução ótima única em

\[
(x_1,x_2)=(0,0).
\]

---

## (k)
Em uma dada iteração do Simplex em Tabelas, se constatarmos que a solução do problema é ilimitada, então pelo menos uma das variáveis não-básicas com custo relativo menor que zero terá sua coluna composta por elementos nulos ou negativos.

**Resposta:**

---

## (l)
Caso o critério de otimalidade do Simplex for alcançado, se obtivermos ao menos uma variável não-básica com custo relativo igual a zero, podemos afirmar que temos múltiplas soluções ótimas.

**Resposta:**

---

## (m)
Se a região factível possui um vértice, então o problema possui solução ótima.

**Resposta:**

---

## (n)
De um modo geral, um problema artificial possui múltiplas soluções ótimas.

**Resposta:**

---

## (o)
Se um PL tem infinitas soluções ótimas, então seu problema artificial possui solução diferente de zero.

**Resposta:**

---

## (p)
Toda solução factível é básica.

**Resposta:**

---

## (q)
Toda solução básica é factível.

**Resposta:**

---

## (r)
Se um problema possui solução ótima, então existe um vértice ótimo.

**Resposta:**

---

## (s)
Existe uma regra de pivoteamento tal que o método Simplex é um algoritmo polinomial para resolver PLs.

**Resposta:**

---

## (t)
Na regra de Bland a ordem das variáveis não é importante, desde que ela seja fixa.

**Resposta:**

---

## (u)
Se o método Simplex entra num ciclo, então uma solução básica degenerada se repete.

**Resposta:**