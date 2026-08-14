# Isogeny

!!! definition "Definition (Isogeny over $K$)"

    Let $K$ be an extension of $K'$.
    Let \(E_1\) and \(E_2\) be elliptic curves over a field \(K'\). An **isogeny** over $K$ is a non-constant [morphism](morphism.md)

    \[
    \phi:E_1\longrightarrow E_2
    \]

    satisfying \(\phi(\mathcal O_{E_1})=\mathcal O_{E_2}\), and represented as a rational map over $K$.

## Degree

!!! definition "Definition (Degree of an isogeny)"

    The **degree** of an isogeny \(\phi:E_1\to E_2\) is the degree of the [induced extension of function fields](../theorems/field_extension_of_morphism.md):

    \[
    \deg\phi=[K(E_1):\phi^*K(E_2)].
    \]

## Related theorems

- [Isogenies preserve the group law](../theorems/isogeny_homomorphism.md)
- [Degree and kernel](../theorems/degree_and_kernel.md)
