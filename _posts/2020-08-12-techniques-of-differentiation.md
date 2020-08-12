---
title: 2.2 Techniques of differentiation
layout: post
---

## Slope of a constant
![](/assets/img/6.1.jpg){: class="mr"}
$m = 0 \Rightarrow \boxed{\dfrac{\partial}{\partial x}[c] = 0}$

\* The deriv. of a constant is $0$

### Examples
$\dfrac{\partial}{\partial x} [3] = 0$

$\dfrac{\partial}{\partial x} [-1] = 0$

<p class="clearfix"></p>

## Derivative of n power
$\boxed{\dfrac{\partial}{\partial x} [x^n] = nx^n-1}$

### Examples
$
\text{1) }\dfrac{\partial}{\partial x} [x^2] = 2x^2-1 = 2x \qquad
\text{2) }\dfrac{\partial}{\partial x} [x^5] = 5x^4 \qquad
\text{3) }\dfrac{\partial}{\partial x} [\frac{1}{x}] = -1x^{-2} \qquad
\text{4) }\dfrac{\partial}{\partial x} [x] = 1$

### Example
\* $\boxed{\dfrac{\partial}{\partial x} [c * f(x)] = c * \dfrac{\partial}{\partial x} [f(x)]}$

$\dfrac{\partial}{\partial x} [5x^4] = 5 * \dfrac{\partial}{\partial x} [x^4] = 5 * 4x^3 = 20x^3$

$\boxed{\dfrac{\partial}{\partial x} [f(x) \pm g(x)] = \dfrac{\partial}{\partial x} [f(x)] \pm \dfrac{\partial}{\partial x} [g(x)]}$

### Example
At what points does $y = x^3 - 3x + 4$ have horizontal tangent lines?

$\dfrac{\partial y}{\partial x} = 3x^2 - 3$ (slope)

\\[3x^2 - 3 = 0 \\]
\\[3(x^2 - 1) = 0 \\]
\\[3(x+1)(x-1) = 0 \\]
\\[x = -1 \qquad x = 1 \\]

## Higher derivatives


|             $1^{st}$             |              $2^{nd}$              |              $3^{rd}$              |
|:--------------------------------:|:----------------------------------:|:----------------------------------:|
|              $f\rq(x)$             |              $f\rq\rq(x)$              |              $f\rq\rq\rq(x)$             |
|               $y\rq$               |                $y\rq\rq$               |               $y\rq\rq\rq$               |
| $\quad\dfrac{\partial y}{\partial x}\quad$ | $\quad\dfrac{\partial^2 y}{\partial x}\quad$ | $\quad\dfrac{\partial^3 y}{\partial x}\quad$ |

### Example
First simplify

\\[y = \dfrac{x^5-2x-3}{3\sqrt{x}} = \dfrac{x^5}{3x^{1 \over 2}} - \dfrac{2x}{3x^{1 \over 2}} - \dfrac{3}{3x^{1 \over 2}} = \dfrac{1}{3}x^{9 \over 2} - \dfrac{2}{3}x^{1 \over 2} - x^{-{1 \over 2}}\\]

and then find a derivative:
\\[\dfrac{\partial y}{\partial x} = \dfrac{3}{2}x^{7 \over 2} - \dfrac{1}{3}x^{-{1 \over 2}} + \dfrac{1}{2}x^{-{3 \over 2}}\\]