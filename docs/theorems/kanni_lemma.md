# Kanni's Lemma

!!! theorem "Theorem (Kanni's Lemma)"

    Let $E, E_a, E_b, E_{ab}$ be elliptic curves over $K$.
    Let $f, g, f', g'$ be isogenies over $\overline{K}$ of degree $d_a = \deg(f) = \deg(f')$
    and degree $d_b = \deg(g) = \deg(g')$ that fit into the following diagram

    \[
    \begin{array}{ccc}
    E & \xrightarrow{\ f\ } & E_a \\
    {\scriptstyle g}\downarrow & & \downarrow{\scriptstyle g'} \\
    E_b & \xrightarrow{\ f'\ } & E_{ab}
    \end{array}
    \]

    and $\gcd(d_a, d_b) = 1$.

    Let $N = d_a + d_b$. Then,

    $$
        \Phi = \begin{pmatrix}
            f & \widehat{g}' \\
            -g & \widehat{f}'
        \end{pmatrix}
    $$

    is an $(N, N)$-isogeny $\Phi : E\times E_{ab} \to E_a \times E_b$ such that

    $$
        \ker\Phi = \langle (-\widehat{g}(P_N), f'(P_N)), (-\widehat{g}(Q_N), f'(Q_N)) \rangle,
    $$
    
    where $E_a[N] = \langle P_N, Q_N \rangle$.

??? proof "Proof"

    (i) $\deg\Phi = d_a + d_b$

    The dual isogeny $\widehat{\Phi}$ is

    $$
        \widehat{\Phi} = \begin{pmatrix}
            \widehat{f} & -\widehat{g}\\
            g' & f'
        \end{pmatrix}.
    $$

    Then, we have

    $$
        \widehat{\Phi} \circ \Phi = \begin{pmatrix}
            \widehat{f}\circ f + \widehat{g}\circ g & \widehat{f} \circ \widehat{g}' - \widehat{g} \circ \widehat{f}'\\
            g'\circ f - f'\circ g & g'\circ \widehat{g}' + f' \circ \widehat{f}'
        \end{pmatrix}
    $$

    By the commutativity $g' \circ f = f' \circ g$, we have

    $$
        \widehat{\Phi} \circ \Phi = \begin{pmatrix}
            [d_a] + [d_b] & 0\\ 0 & [d_a] + [d_b]
        \end{pmatrix} = [N]I_2.
    $$

    This implies that $\deg\Phi = (N, N)$.

    (ii) $\ker\Phi =  \langle (-\widehat{g}(P_N), f'(P_N)), (-\widehat{g}(Q_N), f'(Q_N)) \rangle$

    For the first point $(-\widehat{g}(P_N), f'(P_N))$, we have
    
    $$
    \Phi((-\widehat{g}(P_N), f'(P_N))) = \begin{pmatrix}
    -f\circ \widehat{g}(P_N) + \widehat{g}' \circ f'(P_N) \\
    g \circ \widehat{g}(P_N) + \widehat{f}' \circ f'(P_N)
    \end{pmatrix} = \begin{pmatrix}
        \mathcal{O} \\ [N]P_N
    \end{pmatrix}
    = \mathcal{O}.
    $$

    For the second point $(-\widehat{g}(Q_N), f'(Q_N))$, we have

    $$
    \Phi((-\widehat{g}(Q_N), f'(Q_N))) = \begin{pmatrix}
    -f \circ \widehat{g}(Q_N) + \widehat{g}' \circ f'(Q_N) \\
    g \circ \widehat{g}(Q_N) + \widehat{f}' \circ f'(Q_N)
    \end{pmatrix} = \begin{pmatrix}
        \mathcal{O} \\ [N]Q_N
    \end{pmatrix}
    = \mathcal{O}.
    $$

    and since

    $$
    \#\langle (-\widehat{g}(P_N), f'(P_N)), (-\widehat{g}(Q_N), f'(Q_N)) \rangle = N^2 = \deg\Phi,
    $$

    This proves the claim.
