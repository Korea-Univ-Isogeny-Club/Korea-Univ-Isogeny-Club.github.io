# The structure of torsion subgroup

!!! theorem "Corollary"

    Let $K$ be a field and $m \in \mathbb{Z}$ with $m\neq 0$. Let $E/K$ be an elliptic curve.

    (a) If either $\mathrm{char}(K) = 0$ or $p=char(K) >0$ and $p \nmid m$, then

    $$
        E[m] \cong \mathbb{Z}/m\mathbb{Z} \times \mathbb{Z}/m\mathbb{Z}.
    $$

    (b) If $\mathrm{char}(K) = p >0$, then one of the following is true:

    (i)

    $$
        E[p^e] = \{O\} \text{ for all } e = 1, 2, 3, \dots
    $$

    (ii)

    $$
        E[p^e] \cong \mathbb{Z}/p^e\mathbb{Z} \text{ for all } e= 1,2,3,\dots
    $$

??? proof "Proof"

    (a)

    The fact that $p \nmid \deg[m] = m^2$ tells us that $[m]$ is a finite separable map.

    Hence, we have

    $$
        \#E[m] = \deg[m] = m^2.
    $$

    Further for every integer $d$ dividing $m$, we similarly have

    $$
        \#E[d] = d^2.
    $$

    It is easy to see that the only possibility is

    $$
        E[m] = \mathbb{Z}/m\mathbb{Z} \times \mathbb{Z}/m\mathbb{Z}.
    $$

    (b)

    Let $\phi$ be the $p$-th power Frobenius morphism. Then

    $$
        \#E[p^e] = \deg_s[p^e] = (\deg_s(\widehat{\phi} \circ \phi))^e = (\deg_s \widehat{\phi})^e.
    $$

    If $\widehat{\phi}$ is inseparable, then $\deg_s\widehat{\phi} = 1$, so

    $$
        \#E[p^e]=1 \text{ for all } e.
    $$

    Otherwise $\widehat{\phi}$ is separable, we have

    $$
        \#E[p^e] = p^e \text{ for all } e.
    $$

    This implies that

    $$
        E[p^e] \cong \mathbb{Z}/p^e\mathbb{Z} \text{ for all } e.
    $$