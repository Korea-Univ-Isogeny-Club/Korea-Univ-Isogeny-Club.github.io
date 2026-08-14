# $K(C_1)$ is a finite extension of $\phi^*(K(C_2))$ 

!!! theorem "Proposition"

    Let $C_1$ be a nonsingular projective variety of dimension one (nonsingular curve) over $K$, let $C_2$ be any projective variety of dimension one (curve) over $K$,
    and let $\phi: C_1 \to C_2$ be a nonconstant [morphism](../definitions/morphism.md). Then,
    $K(C_1)$ is a finite extension field of $\phi^*(K(C_2))$.

??? proof "Proof"

    We have

    $$
        \phi^*(K(C_2)) \subset K(C_1)
    $$

    and, since $\phi$ is surjective, both $\phi^*(K(C_2))$ and $K(C_1)$ have
    transcendence degree 1 of $K$.

    Thus, $K(C_1)$ must be a finite algebraic extension of $\phi^*(K(C_2))$.

## Reference
+ Joseph H. Silverman, "The Arithemtic of Elliptic Curves" (II.2.4), p.20
+ Robin Hartshorne, "Algebraic Geometry" (II.6.8), p.137