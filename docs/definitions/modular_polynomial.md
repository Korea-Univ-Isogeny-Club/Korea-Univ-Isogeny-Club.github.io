# Modular Polynomial

!!! definition "Definition (Modular Polynomial)"

    Let $\ell \in \mathbb{N}$, and $p$ a prime with $p \neq \ell$.

    A modular polynomial $\Phi_\ell \in \mathbb{Z}[X,Y]$ is a polynomial
    such that

    $$
        \overline{\Phi}_\ell(x,y) = 0,
    $$

    if and only if there exists two elliptic curves $E_1, E_2$ over $\overline{\mathbb{F}}_p$ such that

    $$
        x = j(E_1)\text{, and } y=j(E_2),
    $$

    where $\overline{\Phi} = \Phi \mod p$.