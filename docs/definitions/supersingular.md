# Supersingular Elliptic Curves

!!! definition "Definition (Supersingular Elliptic Curves)"

    Let $\mathbb{F}_q$ be a field with $\mathrm{char}(\mathbb{F}_q) = p > 0$, and let $E/\mathbb{F}_q$ be an elliptic curve.
    $E/\mathbb{F}_q$ is **supersingular** if one of the following conditions holds

    (i) $E[p^r] = 0$ for all $r \geq 1$.

    (ii) The dual of $p^r$-power Frobenius map is purely inseparable for all $r \geq 1$.

    (iii) The endomorphism $[p] : E \to E$ is purely inseparable and $j(E) \in \mathbb{F}_{p^2}$.

    (iv) $\mathsf{End}(E)$ is a maximal order in a quaternion algebra.

    (v) The trace of Frobenius is divisible by $p$.

!!! theorem "Corollary"

    For a prime $p$, if $E/\mathbb{F}_{p^r}$ is supersingular for some positive integer $r$, then
    $E/\mathbb{F}_{p^n}$ is supersingular for all $n \geq r$. 

!!! theorem "Corollary"

    Let $p \geq 5$ be a prime.

    Let $E/\mathbb{F}_{p}$ is supersingular. Then

    $$
        \#E(\mathbb{F}_{p^n}) = \begin{cases}
           p^n + 1 & \text{if } n \text{ is odd} \\
           (p^{n/2} - (-1)^{n/2})^2 & \text{if } n \text{ is even}
        \end{cases}
    $$

??? proof "Proof"

    By the [property of the trace of Frobenius](trace_of_frobenius.md), let's denote

    $$
        \#E(\mathbb{F}_{p^n}) = p^n - a_n + 1.
    $$

    Let $\phi : E(\overline{\mathbb{F}}_p) \to E(\overline{\mathbb{F}}_p)$ be the
    $p$-power Frobenius endomorphism.

    Let $\ell$ be a prime different from $p$, and $T_\ell(E)$ be the [Tate module](tate_module.md).

    Let $\alpha, \beta$ be the eigenvalues of $\phi$ on $T_\ell(E)$.

    Then, $\alpha^n, \beta^n$ are the eigenvalues of $\phi^n$, and we have

    $$
        \alpha^n + \beta^n = a_n.
    $$

    From the characteristic polynomial of $\phi$:

    $$
        x^2 - a_1 x + p = 0,
    $$

    we have 
    
    $$
        (\alpha^{n+2} + \beta^{n+2}) - a_1(\alpha^{n+1} + \beta^{n+1}) + p(\alpha^n + \beta^n)
        = a_{n+2} - a_1 a_{n+1} + p a_n = 0.
    $$

    (i) By [Hasse's theorem](../theorems/hasse_theorem.md),

    $$
        \#E(\mathbb{F}_p) = p + 1, a_1 = 0
    $$

    and, since $E(\mathbb{F}_p)$ is a subgroup of $E(\mathbb{F}_{p^2})$ and both are abelian groups, we have

    $$
        \#E(\mathbb{F}_p) | \#E(\mathbb{F}_{p^2}).
    $$

    By [Hasse's theorem](../theorems/hasse_theorem.md) and the condition $p \geq 5$, we have

    $$
        \#E(\mathbb{F}_{p^2}) = (p+1)^2, a_2 = 2p
    $$

    (ii) We have recurrence relation

    $$
        a_{n+2} = -p a_n.
    $$

    Thus, we have

    $$
        a_n = \begin{cases}
            0 & \text{if } n \text{ is odd}\\
            2(-p)^{n/2}  & \text{if } n \text{ is even}
        \end{cases}
    $$

    This proves the claim.

# References
+ Joseph H. Silverman, "The Arithmetic of Elliptic Curves", V.3.1 (p.145), Exercise 5.10 (p.154)