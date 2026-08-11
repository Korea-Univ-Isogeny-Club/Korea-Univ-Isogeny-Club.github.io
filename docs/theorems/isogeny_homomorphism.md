# Isogenies Preserve the Group Law

!!! theorem "Theorem"

    Every isogeny \(\phi:E_1\to E_2\) is a group homomorphism. In particular,

    \[
    \phi(P+Q)=\phi(P)+\phi(Q)
    \]

    for all \(P,Q\in E_1(\overline K)\).

??? proof "Proof"

    Consider the morphism

    \[
    F(P,Q)=\phi(P+Q)-\phi(P)-\phi(Q).
    \]

    The rigidity lemma shows that \(F\) is constant. Evaluating at \((\mathcal O,\mathcal O)\) gives \(F=\mathcal O\), and hence \(\phi(P+Q)=\phi(P)+\phi(Q)\).

## Related definitions

- [Elliptic curve](../definitions/elliptic_curve.md)
- [Isogeny](../definitions/isogeny.md)
