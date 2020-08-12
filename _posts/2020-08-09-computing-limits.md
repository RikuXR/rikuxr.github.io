---
title: 1.2 Computing Limits
layout: post
categories: [Limits and Continuity]
---

## Basics:

1. $lim_{x \to a} C = C$ (c = constant)
2. $lim_{x \to a} x = a$
3. $lim_{x \to 0^-} \frac{1}{x} = -\infty \quad\ lim_{x \to 0^+} \frac {1}{x} = +\infty$

{:refdef: .image-center}
![](/assets/img/2.1.jpg#inline3)
![](/assets/img/2.2.jpg#inline3)
{: refdef}

## Properties:
$lim_{x \to a} f(x) = L_1 \quad lim_{x \to a} g(x) = L_2$

1. $lim_{x \to a} [f(x) \pm g(x)] = lim_{x \to a} f(x) \pm lim_{x \to a} g(x)$
2. $lim_{x \to a} [f(x) * g(x)] = lim_{x \to a} f(x) * lim_{x \to a} g(x)$
3. $lim_{x \to a} [\frac{f(x)}{g(x)}] = \frac{lim_{x \to a} f(x)}{lim_{x \to a} g(x)}$
4. $lim_{x \to a} [f(x)]^n = [lim_{x \to a} f(x)]^n \longrightarrow  lim_{x \to a} \sqrt[n]{f(x)} = \sqrt[n]{lim_{x \to a} f(x)}$

### Example
$lim_{x \to 2} (x^3-2x+7) = \lim_{x \to 2} x^3 - lim_{x \to 2} 2x + lim_{x \to 2} 7 = 2^3 - 2*2 + 7 = 11$ \
$f(2) = 11 \longleftarrow$ works for any polynomial

\* $lim_{x \to a} P(x) = P(a)$ To find the limit of a polynomial, just plug-in the value

### Example
$lim_{x \to 2} \frac{4x^2 + 1}{x-3} = \frac{4*2^2 + 1}{2-3} = -17$

### Example
![](/assets/img/2.3.jpg){: class="mr"}
$lim_{x \to 5} \frac{x^2-3x-10}{x^2-10x+25} = lim_{x \to 5} \frac{(x-5)(x+2)}{(x-5)(x-5)} = lim_{x \to 5} \frac{x+2}{x-5} = D.N.E.$

Note:
1. If $\frac{0}{0}$, factor & simplilfy
2. If you can't cancel the "Problem", check with "Sign Analysis" because limit might not exist

### Example
$lim_{x \to 1} \frac{x-1}{\sqrt{x} - 1} * \frac{\sqrt{x} + 1}{\sqrt{x} + 1} = lim_{x \to 1} \frac{(x-1)(\sqrt{x} + 1)}{x-1} = lim_{x \to 1}(\sqrt{x} + 1) = \\ \sqrt{1} + 1 = 2$

<p class="clearfix"></p>

## Piece-wise limits
Find 1-sided limits and see if they're equal

![](/assets/img/2.4.jpg){: class="mr"}
### Example
$f(x) = \begin{cases} 
\dfrac{1}{x+2}, \quad x < -2 \cr[1em]
x^2-5,         \quad -2 < x \leq 3 \cr[0.5em]
\sqrt{x+13},   \quad x > 3
\end{cases}
$

$lim_{x \to -2^-} \frac{1}{x+2} = -\infty \quad\quad\quad lim_{x \to 3^-} (x^2-5) = 4$

$lim_{x \to -2^+} (x^2-5) = -1 \quad\quad lim_{x \to 3^+} \sqrt{x+13} = 4$

$lim_{x \to -2} f(x)=D.N.E \quad\quad lim_{x \to 3} x^2-5 = 4$

<p class="clearfix"></p>

## Limits of trig. functions
\* $sin(x)$ & $cos(x)$ are continuous everywhere

$lim_{x \to a} sin(x) = sin(a) \quad\quad lim_{x \to a} cos(x) = cos(a)$

### What about $tan(x)$?

$lim_{x \to a} tan(x) = lim_{x \to a} \frac{sin(x)}{cos(x)} = \frac{lim_{x \to a} sin(x)}{lim_{x \to a} cos(x)} = \frac{sin(a)}{cos(a)} = tan(a), \quad cos(a) \neq 0 \rightarrow x \neq \pm\frac{\pi}{2} + \pi n$

### Example
$lim_{x \to 1} cos(\frac{x^2-1}{x-1}) = cos[lim_{x \to 1} \frac{x^2-1}{x-1}] = 
cos[lim_{x \to 1} (x+1)] = cos(2)$

### Example
$lim_{x \to \frac{\pi}{2}} [3x^2 + cos(x)] = 3(\frac{\pi}{2})^2 + cos(\frac{\pi}{2}) = \frac{3\pi^2}{4}$

### Example
![](/assets/img/2.5.jpg){:class="mr"}
$lim_{x \to 0} [\frac{sin(x)}{x}] = ?$

AREAS:

$\begin{rcases}
   &\text{Big} \triangle = \dfrac{1 * tan(x)}{2} \cr[1em]
   &\text{Sector}  = \dfrac{1 * x}{2} \cr[1em]
   &\text{Small} \triangle = \dfrac{1 * sin(x)}{2}
\end{rcases} \Rightarrow \dfrac{sin(x)}{2} < \dfrac{x}{2} < \dfrac{tan(x)}{2}$

<p class="clearfix"></p>

### Using squeeze theorem
\\[ \dfrac{sin(x)}{sin(x)} < \dfrac{x}{sin(x)} < \dfrac{tan(x)}{sin(x)} \\]
\\[ 1 < \dfrac{x}{sin(x)} < \dfrac{tan(x)}{sin(x)} \\]
\\[ 1 < \dfrac{x}{sin(x)} < \dfrac{1}{cos(x)} \\]
\\[ 1 > \dfrac{sin(x)}{x} > cos(x) \\]

\\[\begin{rcases}
   lim_{x \to 0} 1 = 1 \cr[1em]
   lim_{x \to 0} cos(x) = 1
\end{rcases} \Rightarrow lim_{x \to 0} \dfrac{sin(x)}{x} = 1\\]