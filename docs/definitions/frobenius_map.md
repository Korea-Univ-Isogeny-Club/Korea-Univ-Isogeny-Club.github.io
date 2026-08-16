# Frobenius map

!!! definition "Definition (Frobenius map)"

    Let $\mathbb{F}_q$ be a finite field with characteristic $p > 0$.
    Let $E/\mathbb{F}_q$ be an elliptic curve over $\mathbb{F}_q$ defined by

    $$
        E : y^2 = f(x),
    $$

    where $f(x)$ is a cubic polynomial.

    Then, **$p^r$-power Frobenius map** is

    $$
        \phi_{p^r} : E \to E^{(p^r)}, (x,y) \mapsto (x^{p^r}, y^{p^r}),
    $$

    where $E^{(p^r)}: y^{2} = x^{3} + a^{p^r}x + b^{p^r}$.

# Reference
+ Joseph H. Silverman, "The Arithmetic of Elliptic Curves", II.2, p.25