# $\mathrm{End}_{\mathbb{F}_p}(E)$ is commutative for a supersingular elliptic curve $E/{\mathbb{F}_p}$

!!! theorem "Theorem"

    Let $p$ be a prime.
    For a supersingular elliptic curve $E/\mathbb{F}_p$,
    
    $$
        \mathrm{End}_{\mathbb{F}_p}(E) \otimes \mathbb{Q} = \mathbb{Q}(\sqrt{-p}),
    $$

    which implies that $\mathrm{End}_{\mathbb{F}_p}(E)$ is commutative.

??? proof "Proof"

    Let $\phi : E\to E$ is an endomorphism defined over $\mathbb{F}_p$.

    Let $\pi_p : E\to E$ be the $p$-power Frobenius endomorphism. Then, we have

    $$
        \phi \circ \pi_p = \pi_p \circ \phi.
    $$

    By the [property of supersingular curves](../definitions/supersingular.md),

    $$
        \mathrm{End}_{\mathbb{F}_p}(E) \otimes \mathbb{Q} = C_{B_{p,\infty}}(\pi_p),
    $$

    where $B_{p,\infty}$ is the quaternion algebra ramified at $p$ and $\infty$, and
    $C_{B_{p,\infty}}(\pi_p)$ is the set of elements in $B_{p,\infty}$ which is commutative with $\pi_p$.

    Since $\pi_p^2 = -p$, we have $C_{B_{p,\infty}}(\pi_p) = \mathbb{Q}(\sqrt{-p})$, which proves the claim. 


# References
+ Christina Delfs and Steven D. Galbraith, "Computing isogenies between supersingular elliptic curves over $\mathbb{F}_p$"