---
title: The Derivative
layout: post
---

$\underbrace{
  f'(x) = lim_{h \to 0} \dfrac{f(x_0 + h) - f(x_0)}{h}
}_{\text{This is a derivative}}$ \* Slope of a curve at a point

### Example
Find $f'(x)$ for $f(x) = 3x + 2$.

$f'(x) = 3$ (because for $y = mx +b$ slope = $m$)

## Differentiability
In order for a derivative to exist a a point, $f'(x)$ must exist.

{:refdef: .image-center}
![](/assets/img/5.1.jpg#inline3)
![](/assets/img/5.2.jpg#inline3)
{:refdef}

Two implications:
1. Can't take a derivative at a "sharp point"
2. ... or where slope is vertical

Note: these functions are non-differentiable only at those specific points.

* If a function is not cont., it is not diff.
* If a function is diff. it is cont. (the opposite is not necessarily true)

## Representations for derivatives
$f'(x) \qquad \dfrac{\partial}{\partial x}[f(x)] \qquad 
y' \qquad \dfrac{\partial y}{\partial x}$

$f'(a) \qquad \dfrac{\partial}{\partial x}[f(x)]\Big&#124;\_{x=a} \qquad y'(a) \qquad \dfrac{\partial y}{\partial x}\Big&#124;\_{x=a}$