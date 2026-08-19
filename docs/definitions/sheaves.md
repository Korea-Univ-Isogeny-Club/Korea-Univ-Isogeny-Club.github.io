# Sheaves

!!! definition "Definition (Presheaf)"

    Let $X$ be a topological space. A **presheaf** $\mathcal{F}$ of abelian group on $X$
    consists of the data

    (a) for every open subset $U \subseteq X$, an abelian group $\mathcal{F}(U)$, and

    (b) (Global $\Rightarrow$ Local) for every inclusion $V \subseteq U$ of open subsets of $X$, a morphism of abelian
    groups $\rho_{UV} : \mathcal{F}(U) \to \mathcal{F}(V)$,

    subject to the conditions

    (i) $\mathcal{F}(\emptyset) = 0$, where $\emptyset$ is the empty set.
    
    (ii) $\rho_{UV}$ is the identity map $\mathcal{F}(U) \to \mathcal{F}(U)$, and

    (iii) if $W \subseteq V \subseteq U$ are three open subsets, then $\rho_{UW} = \rho_{VW} \circ \rho_{UV}$.

!!! definition "Definition (Sheaf)"

    A presheaf $\mathcal{F}$ on a topological space $X$ is a **sheaf** if it satisfies the
    following supplementary conditions:

    (iv) (Local $\Rightarrow$ Global) if $U$ is open set, if $\{V_i\}$ is an open covering of $U$, and if $s\in \mathcal{F}(U)$ is
    an element such that $s|_{V_i} = 0$ for all $i$, then $s=0$.

    (v) (Local $\Rightarrow$ Global) if $U$ is open set, if $\{V_i\}$ is an open covering of $U$, and if we have
    elements $s_i \in \mathcal{F}(V_i)$ for each $i$, with the property that for each $i,j$, $s_i|_{V_i \cap V_j} = s_j|_{V_i \cap V_j}$,
    then there is an element $s \in \mathcal{F}(U)$ such that $s|_{V_i} = s_i$ for each $i$.

# References
+ Robin Hartshorne, "Algebraic Geometry", II, p.61