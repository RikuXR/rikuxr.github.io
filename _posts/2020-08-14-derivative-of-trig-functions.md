---
title: 2.5 Finding Derivatives of Trigonometric Functions
layout: post
categories: Derivatives
---

## Derivative of sin
$lim_{h \to 0} \dfrac{sin(x)}{x} = 1 \qquad lim_{h \to 0} \dfrac{1 - cos(x)}{x} = 0$

$f(x) = sin(x)$ find $f\rq(x)$

$\begin{aligned}
  f\rq(x) = lim_{h \to 0} \dfrac{sin(x + h) - sin(x)}{h} &= 
  lim_{h \to 0} \dfrac{sin(x)cos(h) + cos(x)sin(h) - sin(x)}{h} = \cr[1em]
  &= lim_{h \to 0} \dfrac{sin(x)cos(h) - sin(x)}{h} + \dfrac{cos(x)sin(h)}{h} = \cr[1em]
  &= lim_{h \to 0} \dfrac{sin(x)(cos(h) - 1)}{h} + cos(x) * \dfrac{sin(h)}{h} = 
  \boxed{cos(x)}
\end{aligned}$

## Derivatives of trigs
$\begin{aligned}
  \dfrac{\partial}{\partial x}[sin(x)] &= cos(x) \qquad
  \dfrac{\partial}{\partial x}[cos(x)] = -sin(x) \cr[1em]
  \dfrac{\partial}{\partial x}[tan(x)] &= sec^2(x) \qquad
  \dfrac{\partial}{\partial x}[sec(x)] = sec(x)tan(x) \cr[1em]
  \dfrac{\partial}{\partial x}[csc(x)] &= -csc(x)cot(x) \qquad
  \dfrac{\partial}{\partial x}[cot(x)] = -csc^2(x) \cr[1em]
\end{aligned}$

### Example
$\dfrac{\partial y}{\partial x}$ for $y = xsin(x)$

$\dfrac{\partial y}{\partial x} = \dfrac{\partial}{\partial x} [x] * sin(x) + x * \dfrac{\partial}{\partial x} [sin(x)] = sin(x) + xcos(x)$

### Example
$y = \dfrac{sin(x)}{1 + cos(x)}$

$\begin{aligned}
  \dfrac{\partial y}{\partial x} = \dfrac{[1 + cos(x)] * \dfrac{\partial}{\partial x} sin(x) -\dfrac{\partial}{\partial x} [1 + cos(x)] * sin(x)}{[1 + cos(x)]^2} &= 
  \dfrac{[1 + cos(x)]cos(x) - sin(x) * [-sin(x)]}{[1 + cos(x)]^2} \cr[1em]
  &= \dfrac{cos(x) + cos^2(x) + sin^2(x)}{[1 + cos(x)]^2} = \dfrac{1 + cos(x)}{[1 + cos(x)]^2}
\end{aligned}$

$\dfrac{\partial y}{\partial x} = \dfrac{1}{1 + cos(x)}$