---
title: 2.3 The Product and Quotient Rules
layout: post
categories: Derivatives
---

## Product rule
$\dfrac{\partial}{\partial x} [f(x) * g(x)] = f'(x) * g(x) + f(x) * g'(x)$

### Example
$\dfrac{\partial}{\partial x} [x^2 * x^3] = \dfrac{\partial}{\partial x} [x^2] * x^3 + x^2 * \dfrac{\partial}{\partial x} [x^3] = 2x * x^3 + x^2 * 3x^2 = 2x^4 + 3x^4 = 5x^4$

### Example
$f(x)=(1+x^2)\sqrt{x}$

$f\rq(x) = \dfrac{\partial}{\partial x} [1 + x^2] * \sqrt{x} + (1 + x^2) * \dfrac{\partial}{\partial x} [\sqrt{x}] = 2x * \sqrt{x} + (1 + x^2) * \dfrac{1}{2\sqrt{x}}$

### Example
$g(x) = (x^2 + 1)f(x) \qquad f(2) = 3 \quad f\rq(2) = -1$

Find $g\rq(2)$

$g\rq(x) = \dfrac{\partial}{\partial x} (x^2 + 1) * f(x) + (x^2 + 1) * \dfrac{\partial}{\partial x} f(x) = 2x * f(x) + (x^2 + 1) * (-1)$

$g\rq(2) = 2 * 2 * 3 - 5 = 7$

## Quotient Rule
$\dfrac{\partial}{\partial x} [\frac{f(x)}{g(x)}] = \dfrac{g(x) * f\rq(x) - g\rq(x) * f(x)}{g(x)^2}$

### Example
$y = \dfrac{x^3 - 3x^2 - 5}{2x + 5}$

$\dfrac{\partial y}{\partial x} = \dfrac{(2x + 5) * \dfrac{\partial}{\partial x} [x^3 - 3x^2 -5] - (x^3 - 3x^2 - 5) * \dfrac{\partial}{\partial x} [2x + 5]}{(2x + 5)^2} = \dfrac{(2x + 5)(3x^2 - 6x) - (x^3 - 3x^2 -5) * 2}{(2x + 5)^2} $

$\dfrac{\partial y}{\partial x} = \dfrac{6x^3 + 15x^2 - 12x^2 - 30x - 2x^3 + 6x^2 + 10}{(2x + 5)^2} = \dfrac{4x^3 + 9x^2 - 30x + 10}{(2x+5)^2}$