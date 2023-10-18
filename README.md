# QAP Assignment

Calculate QAP step by step for the given equation. Fill in the values in this markdown to complete the assignment

$$
x^2-x-42 == 0
$$

## Gates

[Add the gates here]

## Symbols

symbols = [~one, x, ?, ?, ?, ?]

## Solution Vector

$\vec{s}$ = [1, 7, ?, ?, ?, ?]

## R1CS

### Gate #1

$$ \vec{a} = [?, ?, ?, ?, ?, ?] $$

$$ \vec{b} = [?, ?, ?, ?, ?, ?] $$

$$ \vec{c} = [?, ?, ?, ?, ?, ?] $$

Verify $$\vec{a}.\vec{s} * \vec{b}.\vec{s} - \vec{c}.\vec{s} == 0$$

### Gate #2

$$ \vec{a} = [?, ?, ?, ?, ?, ?] $$

$$ \vec{b} = [?, ?, ?, ?, ?, ?] $$

$$ \vec{c} = [?, ?, ?, ?, ?, ?] $$

Verify $$\vec{a}.\vec{s} * \vec{b}.\vec{s} - \vec{c}.\vec{s} == 0$$

### Gate #3

$$ \vec{a} = [?, ?, ?, ?, ?, ?] $$

$$ \vec{b} = [?, ?, ?, ?, ?, ?] $$

$$ \vec{c} = [?, ?, ?, ?, ?, ?] $$

Verify $$\vec{a}.\vec{s} * \vec{b}.\vec{s} - \vec{c}.\vec{s} == 0$$

### Gate #4

$$ \vec{a} = [?, ?, ?, ?, ?, ?] $$

$$ \vec{b} = [?, ?, ?, ?, ?, ?] $$

$$ \vec{c} = [?, ?, ?, ?, ?, ?] $$

Verify $$\vec{a}.\vec{s} * \vec{b}.\vec{s} - \vec{c}.\vec{s} == 0$$

## Constraint Matrices

$$
A = \begin{bmatrix}
? & ? & ? & ? & ? & ? \\
? & ? & ? & ? & ? & ? \\
? & ? & ? & ? & ? & ? \\
? & ? & ? & ? & ? & ? \\
\end{bmatrix}
$$

$$
B = \begin{bmatrix}
? & ? & ? & ? & ? & ? \\
? & ? & ? & ? & ? & ? \\
? & ? & ? & ? & ? & ? \\
? & ? & ? & ? & ? & ? \\
\end{bmatrix}
$$

$$
C = \begin{bmatrix}
? & ? & ? & ? & ? & ? \\
? & ? & ? & ? & ? & ? \\
? & ? & ? & ? & ? & ? \\
? & ? & ? & ? & ? & ? \\
\end{bmatrix}
$$

## QAP

$$
A(x) = \begin{bmatrix}
?x^3 + ?x^2 + ?x + ?
\\
?x^3 + ?x^2 + ?x + ?
\\ 
?x^3 + ?x^2 + ?x + ? \\ 
?x^3 + ?x^2 + ?x + ? \\ 
?x^3 + ?x^2 + ?x + ? \\
?x^3 + ?x^2 + ?x + ? \\
\end{bmatrix}
$$

$$
B(x) = \begin{bmatrix}
?x^3 + ?x^2 + ?x + ?
\\
?x^3 + ?x^2 + ?x + ?
\\ 
?x^3 + ?x^2 + ?x + ? \\ 
?x^3 + ?x^2 + ?x + ? \\ 
?x^3 + ?x^2 + ?x + ? \\
?x^3 + ?x^2 + ?x + ? \\
\end{bmatrix}
$$

$$
C(x) = \begin{bmatrix}
?x^3 + ?x^2 + ?x + ?
\\
?x^3 + ?x^2 + ?x + ?
\\ 
?x^3 + ?x^2 + ?x + ? \\ 
?x^3 + ?x^2 + ?x + ? \\ 
?x^3 + ?x^2 + ?x + ? \\
?x^3 + ?x^2 + ?x + ? \\
\end{bmatrix}
$$

$$A(x).\vec{s} = ?$$
$$B(x).\vec{s} = ?$$
$$C(x).\vec{s} = ?$$

$$A(x).\vec{s} * B(x).\vec{s} - C(x).\vec{s} = ?$$

Since the above polynomial is equal to $H(x).Z(x)$ it should have roots at x = 1, 2, 3, 4. Verify the same by pasting the polynomial [here](https://www.wolframalpha.com/).

## Evaluation

-   Clone this template repo, by clicking on `Use this template` and then selecting `Create a new repository`

-   Give a name to this repo and set visibility to `Private`

-   Add us as collaborators

    * Go to the Settings tab
    * Select Collaborators from the left pane
    * Click Add People
    * Add username `shubham-kanodia` as a collaborator

-   Clone the repo you just created

    ```
    git clone CLONE_URL
    ```
    
-   Create a new branch with your name. You can use the following command

    ```
    git checkout -b my-name
    ```

-   Complete the assignment

-   Create a pull request from your branch to the main branch of the repo

-   Since this assignment is manually evaluated we will provide feedback on your solution in form of pull request comments
