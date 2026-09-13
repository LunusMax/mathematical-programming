# Exercício 10

Descreva as ideias por trás do Método Simplex. Em que se baseia este método? Por que a condição de que a região factível

```math
S = \{x \in \mathbb{R}^n;\; Ax = b,\; x \geq 0\}
```

seja convexa é importante para o bom funcionamento do método?

**Resposta:**

O Método Simplex é um algoritmo que percorre os vértices da região factível, passando de uma solução básica factível para outra que melhora a função objetivo.

A convexidade é importante, pois garante que, se existir uma solução ótima finita, existe pelo menos uma solução ótima em um vértice da região factível. Dessa forma, o Simplex pode buscar a solução ótima percorrendo os vértices da região factível.