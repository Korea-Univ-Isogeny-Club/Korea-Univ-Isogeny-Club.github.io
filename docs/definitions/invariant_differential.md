# Invariant Differential

!!! definition "Definition (invariant differential)"

    Let $E/K$ be an elliptic curve given by the usual Weierstrass equation

    $$
        E: y^2 + a_1xy + a_3y = x^3 + a_2x^2 + a_4x + a_6.
    $$

    The differential

    $$
        \omega = \frac{dx}{2y + a_1x + a_3}
    $$

    has neither zeros nor poles. It is called **invariant differential**.

!!! theorem "Proposition"

    Let $\omega$ is the invariant differential of an elliptic curve $E$.

    Let $Q \in E$ and let $\tau_Q : E \to E$ be the translation-by-$Q$ map. Then

    $$
        \tau_Q^*\omega = \omega.
    $$