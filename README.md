# many-maps
Magma code related to finding pairs (C,E), where E is an elliptic curve and C is a genus-2 curve with maps of every degree n>1 to E.

This code is related to the paper

[Howe2026] Everett W. Howe: [Curves of genus two with maps of every degree to a fixed elliptic curve](https://doi.org/10.48550/arXiv.2601.19050).


ManyMaps.magma contains the main programs to reproduce the computations in [Howe2026]. Running

    CurvesWithManyMaps();
   
will reproduce information in Proposition 12 and in Table 1 of [Howe2026].

Examples.magma contains code to verify Example 15 in Section 5 of [Howe2026]. Running

    VerifyManyMaps()
   
will show equation (8) does hold. It also contains explicit formulas for similar examples.

Intersection.magma contains code to verify that if q is a positive definite integer ternary quadratic form that does not represent 1, then there is an n with 1 < n < 1812 such that q does not primitively represent n^2. (This is Proposition 17 from [Howe2026]). Running

    runthroughforms()

will verify this. Running

    sharp()

will verify that the upper bound is sharp. In particular, it checks that the form 4x^2 + 9y^2 + 15z^2 + 2xy + 3xz + 8yz does not represent 1, but primitively represents every n^2 with 1 < n < 1811.

modpols61.magma includes a program that will return a list of the first 61 classical modulat polynomials.
