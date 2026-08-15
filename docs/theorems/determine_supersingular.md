# Determining whether an elliptic curve is supersingular

!!! theorem "Theorem"

    Let $\mathbb{F}_q$ be a finite field of characteristic $p \geq 3$.

    Let $E/\mathbb{F}_q$ be an elliptic curve given by a Weierstrass equation

    $$
        E: y^2 = f(x),
    $$

    where $f(x) \in \mathbb{F}_q[x]$ is a cubic polynomial with distinct roots in $\overline{\mathbb{F}}_q$.
    Then $E$ is [supersingular](../definitions/supersingular.md) if and only if the coefficient of $x^{p-1}$ in $f(x)^{\frac{p-1}{2}}$ is zero.

??? proof "Proof"

    The number of points of $E$ is

    $$
        \#E(\mathbb{F}_q) = 2\times \#\{x \in \mathbb{F}_q: \exists y \text{ such that } y^2 = f(x)\} + 1.
    $$

    Adding one is for the point at infinity. Using Euler's criterion, we have

    $$
        \#E(\mathbb{F}_q) \equiv 1 + \sum_{x \in \mathbb{F}_q} f(x)^{\frac{q-1}{2}} \mod q.
    $$

    Using the cyclic nature of $\mathbb{F}_q^*$, we have

    $$
        \sum_{x \in \mathbb{F}_q} x^i = \begin{cases}
            -1 & \text{if } q-1 | i\\
            0 & \text{if } q-1 \nmid i
        \end{cases}.
    $$

    Since $f(x)$ is a polynomial of degree 3, if we expand $f(x)^{\frac{p-1}{2}}$, we see that
    the expansion has terms of the form $x^n$ for $0 \leq n \leq \frac{3}{2}(q-1)$.
    Hence when we sum over $x \in \mathbb{F}_q$, the only nonzero term comes from $x^{q-1}$.

    Thus if we let

    $$
        A_q = \text{coefficient of } x^{q-1} \text{ in } f(x)^{\frac{q-1}{2}},
    $$

    then

    $$
        \#E(\mathbb{F}_q) \equiv 1-A_q \mod q.
    $$

    According to the [property of supersingular elliptic curves](../definitions/supersingular.md),

    $$
        A_q = 0 \Leftrightarrow a \equiv 0 \mod p,
    $$

    where $a$ is the [trace of Frobenius](../definitions/trace_of_frobenius.md).

    This proves that

    $$
        A_q = 0 \text{ in } \mathbb{F}_q \Leftrightarrow E \text{ is supersingular}.
    $$

    It remains to show that $A_q = 0$ if and only if $A_p = 0$. Writing

    $$
        f(x)^{\frac{p^{r+1}-1}{2}} = f(x)^{\frac{p^r-1}{2}}\left(f(x)^{\frac{p-1}{2}}\right)^{p^r}
    $$

    and equating coefficients yields

    $$
        A_{p^{r+1}} = A_{p^r} A_{p}^{p^r}.
    $$

    An easy induction on $r$ gives the desired result.

!!! theorem "Corollary"

    Let $\mathbb{F}_q$ be a finite field of characteristic $p \geq 3$.

    Let $E/\mathbb{F}_q$ be an elliptic curve given by a Weierstrass equation

    $$
        E: y^2 = x^3 + x
    $$

    Then, $E$ is [supersingular](../definitions/supersingular.md) if and only if $p \equiv 3 \mod 4$.

??? proof "Proof"

    The coefficient of $x^{p-1}$ in the polynomial $(x^3 + x)^{\frac{p-1}{2}}$ is
    the coefficient of $x^{\frac{p-1}{2}}$ in the polynomial $(x^2 + 1)^{\frac{p-1}{2}}$.

    This coefficient is equal to $0$ if $p \equiv 3 \mod 4$, and $\binom{(p-1)/2}{(p-1)/4}$ if $p \equiv 1 \mod 4$.
    Hence, $E$ is supersingular if and only if $p\equiv 3\mod 4$.

# References
+ Joseph H. Silverman, "The Arithmetic of Elliptic Curves", V.4.1(a)