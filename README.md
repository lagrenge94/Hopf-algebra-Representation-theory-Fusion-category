# Hopf-algebras-Representation-theory-and-Fusion-categories
A Mathematica package developed for mathematical physics research involving Hopf algebras, representation theory, and fusion categories. 
This package was originally developped to support my research direction in R-parastatistics [Nature 637, 314-318 (2025), arXiv:2412.13360] and Hopf algebra solvable unitary circuits [Phys. Rev. B 111 (10), 104315 (2025)], but can also be used more broadly for studying topological order and generalized symmetry.

The folder Kernel contains all the package files. This includes three core parts:
  HAConstructor.wl: basic tools for finite dimensional Hopf algebras;
  RepresentationTheory.wl: basic tools in representation theory, with an emphasis on representation of finite groups and (semi-simple) Hopf algebras;
  FusionCategory.wl: basic tools for fusion category, with an emphasis on the category of representations of groups and Hopf algebras.
along with several auxiliary parts:
  AlgebraGenerate.wl: tools for generating an algebraic structure (e.g. groups, algebras, Lie-algebras) from a few given elements;
  FiniteGroups: tools for studying finite groups--mostly unfinished;
  TensorTools.wl: basic tools for tensor network manipulations;
  RmatrixTools.wl: tools for studying solutions to the constant Yang-Baxter equations (R-matrices), with an emphasis on the involutive case;
and some specialized files developped alongside papers:
  ParaspinModel.wl: tools for constructing the local operators and tensors used in the quantum spin models hosting emergent paraparticles in [Nature 637, 314-318 (2025)];
  HAQCATools.wl: tools for studying the Hopf algebra solvable unitary circuits introduced in [Phys. Rev. B 111 (10), 104315 (2025)];

The folder HALibrary stores a collection of finite dimensional (weak) C*-Hopf algebras, including their structure data, representations and corepresentations. File naming convention: if the name of a Hopf algebra is HAname, then HAnameData.mx stores its structure data while HAnameReps.mx stores its representations, and in the code it is loaded by LoadHA["HAName"]. Hopf algebra naming convention: the starting letter indicates how it is constructed:
  (1). "C" means group algebra, e.g. CA5 means C[A5], the group algebra of the alternating group A5. Group naming: 
    Dn for dihedral group of order 2n;
    Dicn for dicyclic group of order 4n;
    An for alternating group of order n!/2;
    Sn for symmetric group of order n!;
    G64: a central type factor group, the group structure behind the set-theoretical R-matrix for the 2D solvable model in [Nature 637, 314-318 (2025), arXiv:2412.13360]
    G36Et: a central type factor group, constructed in Example 4.3 of Math. Res. Lett. 5, 551 (1998)

  (2). "D" means Drinfeld double, e.g. DA4 means D(A4), the Drinfeld double of A4;
  (3). "H" means generally non-commutative non-cocommutative Hopfa algebras, constructed using various techniques;
  (4). "Fibonacci" refers to the 13-dimensional C*-weak Hopf algebra first constructed in Lett Math Phys 38, 437–456 (1996). This is the only proper WHA so far included in this package;
  (5). the suffix (MQHA)MTHA means minimal (quasi)triangular Hopf algebra (D.E.Radford'93), e.g. H20DMQHA.

The folder Examples contains example notebook files, along with several dictionaries for commonly used fusion categories. 
  The file "CommonlyUsedCommands_HA-FC-RT.nb" gathers commonly used commands;
  The file "[arXiv:2412.13360]Paraparticles_SFC_Construction.nb" accompanies the paper arXiv:2412.13360.
  
The package is still at an early stage of development, and will be updated regularly. 
  
