# QAP Assignment

Calculate QAP step by step for the given equation. Fill in the values in this markdown to complete the assignment

$$
x^2-x-42 == 0
$$

## Gates

* $x * x = sym_1$
* $x * -1 = sym_2$
* $sym_1 + sym_2 = sym_3$
* $-42 + sym_3 = out$

## Symbols

symbols = $\vec{s} = [1, x, out, sym_1, sym_2, sym_3]$

## Solution Vector

$\vec{s}$ = [1, 7, 0, 49, -7, 42]

## R1CS

### Gate #1

$$ \vec{a} = [0, 1, 0, 0, 0, 0] $$

$$ \vec{b} = [0, 1, 0, 0, 0, 0] $$

$$ \vec{c} = [0, 0, 0, 1, 0, 0] $$

Verify $$\vec{a}.\vec{s} * \vec{b}.\vec{s} - \vec{c}.\vec{s} == 0$$

### Gate #2

$$ \vec{a} = [0, 1, 0, 0, 0, 0] $$

$$ \vec{b} = [-1, 0, 0, 0, 0, 0] $$

$$ \vec{c} = [0, 0, 0, 0, 1, 0] $$

Verify $$\vec{a}.\vec{s} * \vec{b}.\vec{s} - \vec{c}.\vec{s} == 0$$

### Gate #3

$$ \vec{a} = [1, 0, 0, 0, 0, 0] $$

$$ \vec{b} = [0, 0, 0, 1, 1, 0] $$

$$ \vec{c} = [0, 0, 0, 0, 0, 1] $$

Verify $$\vec{a}.\vec{s} * \vec{b}.\vec{s} - \vec{c}.\vec{s} == 0$$

### Gate #4

$$ \vec{a} = [1, 0, 0, 0, 0, 0] $$

$$ \vec{b} = [-42, 0, 0, 0, 0, 1] $$

$$ \vec{c} = [0, 0, 1, 0, 0, 0] $$

Verify $$\vec{a}.\vec{s} * \vec{b}.\vec{s} - \vec{c}.\vec{s} == 0$$

## Constraint Matrices

$$
A = \begin{bmatrix}
0 & 1 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 & 0 \\
1 & 0 & 0 & 0 & 0 & 0 \\
1 & 0 & 0 & 0 & 0 & 0 \\
\end{bmatrix}
$$

$$
B = \begin{bmatrix}
0 & 1 & 0 & 0 & 0 & 0 \\
-1 & 0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 1 & 1 & 0 \\
-42 & 0 & 0 & 0 & 0 & 1 \\
\end{bmatrix}
$$

$$
C = \begin{bmatrix}
0 & 0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 & 0 & 0 \\
\end{bmatrix}
$$

## QAP

$$
A(x) = \begin{bmatrix}
\frac{-1}{3}x^3 + \frac{5}{2}x^2 - \frac{31}{6}x + 3
\\
\frac{1}{3}x^3 - \frac{5}{2}x^2 + \frac{31}{6}x + -2
\\ 
0 \\ 
0 \\ 
0 \\
0 \\
\end{bmatrix}
$$

$$
B(x) = \begin{bmatrix}
\frac{-15}{2}x^3 + 46x^2 - \frac{173}{2}x + 48
\\
\frac{-1}{6}x^3 + \frac{3}{2}x^2 - \frac{13}{3}x + 4
\\ 
0 \\ 
\frac{-1}{2}x^3 + \frac{7}{2}x^2 - 7x + 4 \\ 
\frac{-1}{2}x^3 + \frac{7}{2}x^2 - 7x + 4 \\
\frac{1}{6}x^3 - x^2 + \frac{11}{6}x - 1 \\
\end{bmatrix}
$$

$$
C(x) = \begin{bmatrix}
0
\\
0
\\ 
\frac{1}{6}x^3 - x^2 + \frac{11}{6}x - 1 \\ 
\frac{-1}{6}x^3 + \frac{3}{2}x^2 - \frac{13}{3}x + 4 \\ 
\frac{1}{2}x^3 - 4x^2 + \frac{19}{2}x - 6 \\
\frac{-1}{2}x^3 + \frac{7}{2}x^2 - 7x + 4 \\
\end{bmatrix}
$$

$$A(x).\vec{s} = 2x^3 - 15x^2 + 31x - 11 $$
$$B(x).\vec{s} = \frac{-68}{3}x^3 + \frac{323}{2}x^2 - \frac{2003}{6}x + 202$$
$$C(x).\vec{s} = \frac{-98}{3}x^3 + \frac{497}{2}x^2 - \frac{3437}{6}x + 406$$

$$A(x).\vec{s} * B(x).\vec{s} - C(x).\vec{s} = \frac{-136}{3}x^6 + 663x^5 - \frac{22757}{6}x^4 + 10700x^3 - \frac{92423}{6}x^2 + 10507x - 2628$$

Since the above polynomial is equal to $H(x).Z(x)$ it should have roots at x = 1, 2, 3, 4. Verify the same by pasting the polynomial [here](https://www.wolframalpha.com/).
