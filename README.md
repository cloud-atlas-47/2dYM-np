# 2dYM-np
Non-perturbative corrections to 2d YM chiral partition function in the large $N$ limit.

## Data files:
- Zholg50q1000.dat: Holomorphic partition function in q-series, from g=1 to g=50, up to q^1000.
- Fholg50mod.dat: Holomorphic free energy, from g=1 to g=50.
- Fnonholg20.dat: Non-holomorphic free energy in almost holomorphic Eisenstein series, from g=1 to g=20.

Format of import:
datalist=ToExpression[Import["datafile","List"]];

Higher order data are available upon resquest.

## Program files:

- Holomorphic Free Energy recursion.nb: Calculate the modular expressions of the holomorphic free energy using the recursion formula from "arXiv:1806.00189 [hep-th]". Output: "Fholg**mod.dat".
- HAE.nb: Calculate non-holomorphic free energy using the HAE from "arXiv:1903.10510 [hep-th]". Input: "Fholg**mod.dat". Output: "Fnonholg**.dat".
- 2dYM-hol-qSer: Calculate the q-series expression of the holomorphic partition function using a highly adapted version of the recursion formula from "arXiv:1806.00189 [hep-th]". Output: "Zholg**q***.dat".
