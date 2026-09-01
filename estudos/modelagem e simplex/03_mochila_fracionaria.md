# Exercício 3 — Problema da Mochila Fracionária

Considere \(n\) objetos que podem ser colocados em um compartimento de capacidade \(c\).
Cada objeto \(i\) possui peso \(p_i\) e valor \(v_i\). É possível selecionar uma fração
entre 0% e 100% de cada objeto.

## Variáveis de decisão

Definimos:

$$
x_i = \text{fração do objeto } i \text{ selecionada}
$$

com:

$$
0 \leq x_i \leq 1, \qquad i = 1, \ldots, n
$$

## Modelo de programação linear

A função objetivo é maximizar o valor total levado:

$$
\max Z = \sum_{i=1}^{n} v_i x_i
$$

sujeito à restrição de capacidade:

$$
\sum_{i=1}^{n} p_i x_i \leq c
$$

e:

$$
0 \leq x_i \leq 1,
\qquad i = 1,\ldots,n
$$

## Interpretação

A variável \(x_i\) representa a proporção do objeto \(i\) que será colocada
no compartimento.

- \(x_i = 0\): o objeto não é selecionado;
- \(x_i = 1\): o objeto é selecionado integralmente;
- \(0 < x_i < 1\): apenas uma fração do objeto é selecionada.

A função objetivo maximiza o valor total dos objetos selecionados, enquanto
a restrição garante que o peso total não ultrapasse a capacidade \(c\).

Como as variáveis \(x_i\) são contínuas no intervalo \([0,1]\), o problema
é um modelo de programação linear conhecido como **problema da mochila
fracionária**.