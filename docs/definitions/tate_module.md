# Tate Module

!!! definition "Definition (Tate Module)"

    Let $E$ be an elliptic curve and let $\ell \in \mathbb{Z}$ be a prime.
    The $\ell$-adic Tate module of $E$ is the group

    $$
        T_\ell(E) = \lim_{n \to \infty} E[\ell^n]
    $$

!!! theorem "Proposition"

    The Tate module has the following structure:

    $$
        T_\ell(E) \cong \mathbb{Z}_\ell \times \mathbb{Z}_\ell \text{ if } \ell \neq \mathrm{char}(K).
    $$

    $$
        T_p(E) \cong \{0\} \text{ or } \mathbb{Z}_p \text{ if } p = \mathrm{char}(K).
    $$

??? proof "Proof"

    Based on the [Corollary about the torsion structure](../theorems/torsion_group_structure.md),
    
    If $\ell \neq \mathrm{char}(K)$,

    $$
        E[\ell^n] \cong \mathbb{Z}/\ell^n\mathbb{Z} \times \mathbb{Z}/\ell^n\mathbb{Z}.
    $$ 

    Thus,

    $$
        \lim_{n \to \infty} E[\ell^n] \cong \lim_{n\to\infty} (\mathbb{Z}/\ell^n\mathbb{Z}) \times \lim_{n\to\infty} (\mathbb{Z}/\ell^n\mathbb{Z}),
    $$

    which is $\mathbb{Z}_\ell \times \mathbb{Z}_\ell$ by definition of $\ell$-adic integers.

    We obtain the second result by following the same way.