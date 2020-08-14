---
title: 2.4 Applications of Derivative
layout: post
categories: Derivatives
---

### DVD Sales Example
DVD sales: $S(t) = \dfrac{7t}{t^2 + 1} \qquad t = years, \quad t \geq 0$

Find:
1. Rate of change for sales \
$S\rq(t) = \dfrac{(t^2 + 1) * \dfrac{\partial}{\partial x} 7t - \dfrac{\partial}{\partial x}(t^2 + 1) * 7t}{(t^2 + 1)^2} = \dfrac{7(t^2 + 1) - 14t^2}{(t^2 + 1)^2} = \dfrac{7t^2 + 7 - 14t^2}{(t^2 + 1)^2} = \boxed{\dfrac{7 - 7t^2}{(t^2 + 1)^2}}$

2. When will sales peak? \
\\[\dfrac{7 - 7t^2}{(t^2 + 1)^2} = 0 \longrightarrow 7(1 - t^2) = 0\\]
\\[\boxed{t = 1 \qquad t \neq -1}\\]

3. How fast will sales increase when movie is releases? (when $t = 0$) \
$S\rq(0) = \dfrac{7 - 7(0)^2}{(0^2 + 1)^2} = 7$

### Example
\\[\underbrace{S = f(t)}\_{\text{a position function}} \qquad 
\underbrace{V(t) = S\rq(t)}\_{\text{velocity}}\\]

\\[\underbrace{a(t) = V\rq(t) = S\rq\rq(t)}\_{\text{acceleration}} \qquad
\underbrace{j(t) = a\rq(t) = S\rq\rq\rq(t)}\_{\text{jerk}}\\]

Find acc. & jerk $S(t) = 2t^3 - 15t^2 + 24t$

$S\rq(t) = 6t^2 - 30t + 24 \newline
S\rq\rq(t) = 12t - 30 = a(t) \newline
S\rq\rq\rq(t) = 12 = j(t)$

### Example
Find max height $S(t) = -16t^2 + 256t$

$V(t) = 0 \newline
V(t) = S\rq(t) = -32t + 256 = 0 \Rightarrow t = 8$

### Cost Example
**Marginal Cost** is $C\rq(x)$ and is the cost of producing an additional item. \
$C(x) = -0.2x^2 + 200x + 9000$

$C\rq(x) = -0.4x + 200 \newline
C\rq(100) = -0.4 * 100 + 200 = 160$ (for item #100)