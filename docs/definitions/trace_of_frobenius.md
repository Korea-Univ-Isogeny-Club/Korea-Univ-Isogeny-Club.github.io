# Trace of Frobenius

!!! definition "Definition (Trace of Frobenius)"

    Let $E/\mathbb{F}_q$ be an elliptic curve. The quantity

    $$
        a = q+1-\#E(\mathbb{F}_q)
    $$

    is called the **trace of Frobenius**.

    It is equal to the trace of the $q$-th power Frobenius map as a linear transformation of $T_\ell(E)$, where $T_\ell(E)$ is the [Tate module](../definitions/tate_module.md) for some prime $\ell$ different from $q$. 

    $$
        \mathrm{tr}(\phi_\ell) = 1 + \deg(\phi) - \deg(1-\phi) = 1 + q - \# E(\mathbb{F}_q) = a.
    $$