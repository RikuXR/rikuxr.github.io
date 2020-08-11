---
title: Continuity
layout: post
---

A curve is continuous if it has no "holes", "breaks" or asymptotes.

Function is continuous at a point "c" if:
 1. $f(c)$ is defined
 2. $lim_{x \to c} f(x)$ must exist
 3. $lim_{x \to c} f(x) = f(c)$

![](/assets/img/3.1.jpg#inline3)
![](/assets/img/3.2.jpg#inline3)
![](/assets/img/3.3.jpg#inline3)

If function is continuous at every point betwen $a$ & $b$, the function is cont. on $(a,b)$.

But what about endpoints?
![](/assets/img/3.4.jpg){: class="mr"}
Cont. on $(a, b]$

In general:
 * Cont. from the left at point C\
 $lim_{x \to c^-} f(x) = f(c)$

 * Cont. from the right at point C\
 $lim_{x \to c^+} f(x) = f(c)$

<p class="clearfix"></p>

### Example
Prove $f(x) = \sqrt{16 - x^2}$ is continuous on $[-4, 4]$

 * Check $(-4, 4)$\
 $lim_{x \to c} f(x) = lim_{x \to c} \sqrt{16-x^2} = \sqrt{16 - c^2} = f(c)$

* $lim_{x \to -4^+} \sqrt{16-x^2} = 0 = f(-4)$

* $lim_{x \to 4^-} \sqrt{16-x^2} = 0 = f(4)$

## Properties: 
$f(x)$ and $g(x)$ are continuous at point "c".

$\begin{rcases}
   &\text{1. } f(x) + g(x) \cr[.5em]
   &\text{2. } f(x) - g(x) \cr[.5em]
   &\text{3. } f(x) * g(x) 
\end{rcases} $ are cont. at point "c"

4\. $\dfrac{f(x)}{g(x)}$ is cont. at "c" unless $g(c) = 0$\
\* If $g(c) = 0$, there is discontinuity at "c"

## Cont. of rational functions
$lim_{x \to c} P(x) = P(c)$

This means:
1. Every polynomial is continuous everywhere

2. A rational function, $\dfrac{P(x)}{Q(x)}$ is cont. everywhere except where denominator is 0. At that point you have a "hole" $\dfrac{0}{0}$ or asymptote $\dfrac{c}{0}$

### Example
$f(x) = \dfrac{x^2-4}{x^2+x-6}$ Find discontinuities
\\[
x^2 + x -6 = 0 \newline
(x+3)(x-2) = 0 \newline
x = -3 \text{ (asymptote)} \quad x = 2 \text{ (hole)}
\\]

## Compositions
If $lim_{x \to c} g(x) = L$ and $f$ is continuous at $L$.
Then $lim_{x \to c} f[g(x)] = f(L) = f(lim_{x \to c} g(x))$\
\* We can separate limits by composition

### Example
$lim_{x \to 4} |10 - 3x^2| = |lim_{x \to 4} (10 - 3x^2)| = |-38| = 38$

* If 2 functions are continuous everywhere their composition is cont. everywhere
* If $f$ is cont. on it's domain, $f^-1$ will also be cont. on its respective domain (range of $f$)

## Intermediate value theorem
{:refdef: .image-center}
![](/assets/img/3.5.jpg#inline3)
![](/assets/img/3.6.jpg#inline3)
{: refdef}

1) $f$ is cont. on $[a, b]$ say k is between $f(a)$ and $f(b)$.\
Then there at least 1 number "c" where "c" is between $a$ and $b$ and $f(c) = k$

2) If $f(a)$ and $f(b)$ have different signs, then there must be at least 1 root on $[a, b]$