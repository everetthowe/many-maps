# many-maps
Magma code related to finding pairs (C,E), where E is an elliptic curve and C is a genus-2 curve with maps of every degree n>1 to E.

This code is related to the paper

[Howe2026] Everett W. Howe: [Curves of genus two with maps of every degree to a fixed elliptic curve](https://doi.org/10.48550/arXiv.2601.19050).


ManyMaps.magma contains the main programs to reproduce the computations in [Howe2026]. Running

    CurvesWithManyMaps();
   
will reproduce information in Proposition 14 and in Table 1 of [Howe2026].

Examples.magma contains code to verify Example 18 in Section 5 of [Howe2026]. Running

    VerifyManyMaps()
   
will show equation (8) does hold. It also contains explicit formulas for similar examples.

Intersection.magma contains code to verify that if q is a positive definite integer ternary quadratic form that does not represent 1 and that does not represent any integer that is 2 or 3 modulo 4, then there is an n in each of the sets D_1 and D_2 (from Theorems 3 and 4) such that q does not primitively represent n^2, thus proving Proposition 21 (and therefore also Theorems 3 and 4). Running

    runthroughforms()

will verify this. Running

    sharp()

will verify the form 4x^2 + 8y^2 + 9z^2 + 4xy + 4yz does not represent 1, but primitively represents every n^2 with 1 < n < 58.

modpols61.magma includes a program that will return a list of the first 61 classical modulat polynomials.
