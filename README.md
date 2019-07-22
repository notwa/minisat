# MiniSat etc.

This repository archives and restores
various versions and derivatives of MiniSat
written by various authors over the years.
[The original MiniSat][homepage] is written and
Copyright © 2003-2006 Niklas Eén, Copyright © 2003-2010 Niklas Sörensson,
and distributed under the terms of [the MIT license.][license_mit]

You may be wondering, [what is MiniSat? What is SAT?](#what-is-this)

## Scripts

* `build-all` — compiles and builds most of the versions here.
This requires git and all of this repository's branches to be cloned.
Note that only Linux is currently supported.

* `check-all` — gathers information about the solvers
  in the `bin` directory created by `build-all`.

## Included Versions

You can download any of the versions on GitHub by following the appropriate link
and clicking on the green "Clone or download" link on the top right.
Select "Download Zip" if you're not familiar with git.

[homepage]: http://minisat.se/MiniSat.html
[master]: https://github.com/notwa/minisat/tree/master
[mp]: https://github.com/notwa/minisat/tree/master-patched
[upstream]: https://github.com/niklasso/minisat/tree/master
[patches]: https://github.com/notwa/minisat/tree/patches
[v220]: https://github.com/notwa/minisat/tree/releases/2.2.0
[v200]: https://github.com/notwa/minisat/tree/releases/2.0.0
[comsps]: https://github.com/notwa/minisat/tree/COMiniSatPS
[ms2glu]: https://github.com/notwa/minisat/tree/minisat-to-glucose
[comsps_archive]: https://web.archive.org/web/20171023151341/http://www.cs.nyu.edu/~chanseok/cominisatps/
[mcomsps]: https://github.com/notwa/minisat/tree/MapleCOMSPS
[mlcm]: https://github.com/notwa/minisat/tree/MapleLCM
[mlcmd]: https://github.com/notwa/minisat/tree/MapleLCMDist
[mlcmdcbt]: https://github.com/notwa/minisat/tree/MapleLCMDistChronoBT
[mlcmdcbtdlv3]: https://github.com/notwa/minisat/tree/MapleLCMDistChronoBTDLv3
[mlcmd_patch]: https://github.com/notwa/minisat/blob/patches/maple-fix-drup-segfault.patch
[license_mit]: https://choosealicense.com/licenses/mit/
[glucose]: https://www.labri.fr/perso/lsimon/glucose/
[glu10]: https://github.com/notwa/minisat/tree/glucose-1.0
[glu20]: https://github.com/notwa/minisat/tree/glucose-2.0
[glu21]: https://github.com/notwa/minisat/tree/glucose-2.1
[glu23]: https://github.com/notwa/minisat/tree/glucose-2.3
[glu30]: https://github.com/notwa/minisat/tree/glucose-3.0
[glu40]: https://github.com/notwa/minisat/tree/glucose-4.0
[glu41]: https://github.com/notwa/minisat/tree/glucose-4.1

### [branch master][master]

This is just a clone of [the upstream master branch.][upstream]

### [branch master-patched][mp]

A version based on [Niklas's most recent work][upstream]
is patched and ready to compile with modern compilers.

### [release 2.2.0][v220]

This is the ubiquitous version of MiniSat
that most of its derivatives are based on.

### [release 2.0][v200]

This is the first release of MiniSat 2
that [glucose-1.0][glu10] is based on.

### Earlier Releases

A few select versions are available on [the MiniSat homepage.][homepage]

### [branch patches][patches]

Various patch files have been archived.
Some of these are used for the build script.

### [branch COMiniSatPS][comsps]

[Chanseok Oh's patches][comsps_archive] have been applied to MiniSat 2.2.0,
essentially turning it into [glucose-2.3.][glu23]

### [branch minisat-to-glucose][ms2glu]

Chanseok Oh's other set of patches have been applied to MiniSat 2.2.0,
behaving similar to [glucose-2.3.][glu23]
This serves as a starting point for MiniSat hack competitions,
in which a limited edit distance is imposed.

### [branch MapleCOMSPS][mcomsps]

Ranking first on the main track of [the 2016 SAT Competition,][comp2016]
this is based on COMiniSatPS.
<!-- TODO: authors? -->

### [branch MapleLCM][mlcm]

This is based on MapleCOMSPS.
<!-- TODO: authors? -->

### [branch MapleLCMDist][mlcmd]

Ranking first on the main track of [the 2017 SAT Competition,][comp2017]
this adds a distance heuristic to MapleLCM,
which in turn is based on MapleCOMSPS.
Note that a patch is available to
[fix a crash in MapleLCMDist's DRUP-outputting code.][mlcmd_patch]
<!-- TODO: authors? -->

### [branch MapleLCMDistChronoBT][mlcmdcbt]

Ranking first on the main track of [the 2018 SAT Competition,][comp2018]
this is based on MapleLCMDist.
<!-- TODO: authors? -->

### [branch MapleLCMDistChronoBTDLv3][mlcmdcbtdlv3]

Ranking first in [the 2019 SAT Race,][race2019]
this is based on MapleLCMDistChronoBT.
<!-- TODO: authors? -->

Note that this appears to be typo'd as MapleLCM**Disc** in the competition.

### [branch glucose-1.0][glu10]

The original Glucose via [the Glucose homepage,][glucose] based on MiniSat 2.0.
Glucose is Copyright © 2009-2017 Gilles Audemard, Laurent Simon.

### [branch glucose-2.0][glu20]

The next Glucose via [the Glucose homepage,][glucose]
based on MiniSat 2.2.0.

### [branch glucose-2.1][glu21]

This is an update to glucose 2.0.
Note that there is a crash specific to this version that has yet to be patched.

### branch glucose-2.2

This version is currently missing.
It was removed from the Glucose homepage.

### [branch glucose-2.3][glu23]

This update to glucose 2.2 was later cleaned up and released as glucose 3.0.
This version was [taken from the 2013 SAT Competition.](http://satcompetition.org/edacc/SATCompetition2013/experiment/22/solver-configurations/862)

Note that this commit is currently missing from
all subsequent branches of Glucose.

### [branch glucose-3.0][glu30]

This is a cleaned up version of Glucose 2.3,
via [the Glucose homepage.][glucose]

This version was used as a base for the Glucose Hack Track of
[the 2016 SAT Competition.][comp2016]

### [branch glucose-4.0][glu40]

This version, also known as Glucose-Syrup,
adds a parallel version of Glucose,
plus some other improvements.

There is an earlier version of 4.0 that is currently absent.

### [branch glucose-4.1][glu41]

This is an incremental improvement over Glucose 4.0.

## Other Versions

These versions have been omitted from this repository
because they are already readily accessible.

[cms]: https://github.com/msoos/cryptominisat
[maple]: https://sites.google.com/a/gsd.uwaterloo.ca/maplesat/

### CryptoMiniSat

[CryptoMiniSat][cms] is a major rewrite of MiniSat, adding many features,
including XOR clauses for improved solving of cryptographic problems.
CryptoMiniSat is written and maintained by [Mate Soos](https://www.msoos.org/)
on [the CryptoMiniSat GitHub repository.][cms]

### More

Some of these versions may later be archived in git branches,
but for the time being, there are:

* [MiniSat derivatives from 2016][solvers2016]
  submitted to [the SAT Competition of 2016.][comp2016]

* [MiniSat derivatives from 2017][solvers2017]
  submitted to [the SAT Competition of 2017.][comp2017]

* [MiniSat derivatives from 2018][solvers2018]
  submitted to [the SAT Competition of 2018.][comp2018]

* [MiniSat derivatives from 2019][solvers2019]
  submitted to [the SAT Race of 2019.][race2019]

* and many more from the [various competitions and races][satcomp]
  held in the past and to be held in the future.

[solvers2016]: https://baldur.iti.kit.edu/sat-competition-2016/solvers/
[solvers2017]: https://baldur.iti.kit.edu/sat-competition-2017/solvers/
[solvers2018]: http://sat2018.forsyte.tuwien.ac.at/solvers/
[solvers2019]: http://sat-race-2019.ciirc.cvut.cz/solvers/
[comp2016]: https://baldur.iti.kit.edu/sat-competition-2016/
[comp2017]: https://baldur.iti.kit.edu/sat-competition-2017/
[comp2018]: http://sat2018.forsyte.tuwien.ac.at/
[race2019]: http://sat-race-2019.ciirc.cvut.cz/
[satcomp]: http://satcompetition.org/

## What is this?

MiniSat is a [SAT solver][SAT] that has been applied to complete
many tasks over the years. SAT is an abbreviation for *satisfiability.*
SAT solvers solve [boolean satisfiability problems,][BSP]
with the possible outcomes of *satisfiable,* *unsatisfiable,*
or *unknown/indeterminate,* often alongside a solution or proof.
SAT problems are [NP-complete.][NP]

SAT solvers also serve as a base for most SMT solvers.
SAT solvers are restricted to problems given in [conjunctive normal form,][CNF]
whereas SMT solvers work with problems described more abstractly.
SMT is an acronym for [Satisfiability Modulo Theories.][SMT]
An example of an SMT solver is the [Simple Theorem Prover (STP),][STP]
which employs a version of MiniSat.

A very informal overview of using SAT and SMT solvers
is given by Dennis Yurichev's [SAT/SMT by Example.][example]
Further information (and slightly dated resources)
is available in [SATLIB — The Satisfiability Library.][satlib]

MiniSat is a popular basis for experimenting with
new ideas to solve problems more efficiently,
due to the software's code being relatively short and simple.
MiniSat's many derivatives have ranked on or won [many competitions,][satcomp]
under many names such as [COMSPS,][comsps_archive] [Glucose,][glucose]
[Maple,][maple] and more.

There are solvers that are not based on MiniSat.
For example, [PicoSAT][picosat] and [yices,][yices]
the latter being an SMT solver.

[SAT]: https://en.wikipedia.org/wiki/Boolean_satisfiability_problem#Algorithms_for_solving_SAT
[BSP]: https://en.wikipedia.org/wiki/Boolean_satisfiability_problem
[NP]: https://en.wikipedia.org/wiki/NP-completeness
[SMT]: https://en.wikipedia.org/wiki/Satisfiability_modulo_theories
[STP]: https://github.com/stp/stp/
[CNF]: https://en.wikipedia.org/wiki/Conjunctive_normal_form
[example]: https://yurichev.com/writings/SAT_SMT_by_example.pdf
[satlib]: https://www.cs.ubc.ca/~hoos/SATLIB/
[picosat]: http://fmv.jku.at/picosat/
[yices]: http://yices.csl.sri.com/
