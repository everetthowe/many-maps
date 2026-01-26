# many-maps
Magma code related to finding pairs (C,E), where E is an elliptic curve and C is a genus-2 curve with maps of every degree n>1 to E.

This code is related to the paper
[Howe2026] Everett W. Howe: Curves of genus two with maps of every degree to a fixed elliptic curve,
arXIv information coming soon.

ManyMaps.magma contains the main programs to reproduce the computations in [Howe2026]. Running

   CurvesWithManyMaps();
   
will reproduce information in Proposition 12 and in Table 1 of [Howe2026]   

Examples.magma contains code to verify Example 15 in Section 5 of [Howe2026]. Running

   VerifyManyMaps()
   
will show equation (8) does hold. We hope to add explicit algebraic models for some of the other curves soon.

modpols61.magma includes a program that will return a list of the first 61 classical modulat polynomials.
