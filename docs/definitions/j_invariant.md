# $j$-invariant

!!! definition "Definition 1 ($j$-invariant)"

    Let $\mathrm{char}(K) \neq 2, 3$.

    Let $E/K$ be an elliptic curve given by

    $$
        E/K : y^2 = x^3 + ax + b
    $$ 

    Then **$j$-invariant** is

    $$
        j(E) = 1728\frac{(4a)^3}{16a^3 + 27b^2}.
    $$

!!! definition "Definition 2 ($j$-invariant)"

    Let $E/K$ be an elliptic curve given by

    $$
        E/K: y^2 + a_1xy + a_3y = x^3 + a_2 x^2 + a_4x + a_6.
    $$

    Then, **j-invariant** is

    $$
        j(E) = 1728 c_4^3 / (c_4^3 - c_6^2),
    $$

    where 

    $$
        b_2 = a_1^2 +4a_2, b_4 = 2a_4 + a_1a_3, b_6 = a_3^2 + 4a_6,
    $$

    $$
        b_8 = a_1^2a_6 + 4a_2a_6 -a_1a_3a_4 + a_2a_3^2 -a_4^2
    $$

    $$
        c_4 = b_2^2 -24b_4,
    $$

    $$
        c_6 = -b_2^3 + 36b_2b_4 - 216b_6
    $$


## $1728$은 어디에서 왔는지?

Ellitpic curve $E$가 정의된 field $K$의 characteristic에 상관 없이 elliptic curve는 Weierstrass equation을 갖는다. $j$-invariant는 isomorphism 변환에 대해 불변량이지만, field $K$의 characteristic이 만약에 2 또는 3 인 경우에, 위 definition에서 항상 $c_4^3 - c_6^2 =0$ 이되어서 j-invariant가 정의되지 않는다.

1728은 소인수분해 하면 $2^6 \times 3^3$이다. 이들은 invariant 값을 계산할때, cubic equation의 차수가 계수에 반영되면서 생긴 값으로 characteristic 2 또는 3 인 경우에도 일관적으로 사용할 수 있게 보정해주어야한다.