# MiniSat etc.

This repository contains various versions and derivatives of MiniSat
written by various authors over the years.
[The original MiniSat][homepage] is written and
Copyright © 2003-2006 Niklas Eén, Copyright © 2003-2010 Niklas Sörensson,
and distributed under the terms of [the MIT license.][license_mit]
You may be wondering, [what is this?](#what-is-this)

## Included Versions

On the [master-patched branch,][mp] a version based on
[Niklas's most recent work][upstream] is patched
and ready to compile with modern compilers.

On the [patches branch,][patches] various patch files have been archived.

The ubiquitous [version 2.2.0 is available here,][v220]
and the earlier [version 2.0 is available here.][v200]
Earlier than that, a few select versions
are available on [the MiniSat homepage.][homepage]

On the [COMiniSatPS branch,][comsps] Chanseok Oh's patches have been applied
to MiniSat 2.2.0. [Visit the COMiniSatPS homepage. (archived)][comsps_archive]
On the [minisat-to-glucose branch,][ms2glu] Chanseok Oh's proof of concept
patches have been applied to MiniSat 2.2.0.

On the [MapleCOMSPS,][mcomsps] [MapleLCMDist,][mlcmd]
and [MapleLCMDistChronoBT][mlcmdcbt] branches, the winners
of the main tracks of SAT Competitions 2016, 2017, and 2018 respectively
have been applied to COMiniSatPS. Note that a patch is available to
[fix a crash in MapleLCMDist's DRUP-outputting code.][mlcmd_patch]

On the [glucose-1.0 branch,][glu10] the original glucose
via [the glucose homepage][glucose] has been applied to MiniSat 2.0.
Similarly, in the remaining glucose branches,
the appropriate glucose versions have been applied to MiniSat 2.2.0:
[glucose-2.0,][glu20]
[glucose-2.1,][glu21]
[glucose-3.0,][glu30]
[glucose-4.0,][glu40] and
[glucose-4.1.][glu41]
Compared to the original releases, some unwanted files
that had slipped in have been removed, and missing licenses have been restored.

You can download any of the versions on GitHub by following the appropriate link
and clicking on the green "Clone or download" link on the top right.
Select "Download Zip" if you're not familiar with git.

[homepage]: http://minisat.se/MiniSat.html
[mp]: https://github.com/notwa/minisat/tree/master-patched
[upstream]: https://github.com/niklasso/minisat/tree/master
[patches]: https://github.com/notwa/minisat/tree/patches
[v220]: https://github.com/notwa/minisat/tree/releases/2.2.0
[v200]: https://github.com/notwa/minisat/tree/releases/2.0.0
[comsps]: https://github.com/notwa/minisat/tree/COMiniSatPS
[ms2glu]: https://github.com/notwa/minisat/tree/minisat-to-glucose
[comsps_archive]: https://web.archive.org/web/20171023151341/http://www.cs.nyu.edu/~chanseok/cominisatps/
[mcomsps]: https://github.com/notwa/minisat/tree/MapleCOMSPS
[mlcmd]: https://github.com/notwa/minisat/tree/MapleLCMDist
[mlcmdcbt]: https://github.com/notwa/minisat/tree/MapleLCMDistChronoBT
[mlcmd_patch]: https://github.com/notwa/minisat/blob/patches/maple-fix-drup-segfault.patch
[license_mit]: https://choosealicense.com/licenses/mit/
[glucose]: https://www.labri.fr/perso/lsimon/glucose/
[glu10]: https://github.com/notwa/minisat/tree/glucose-1.0
[glu20]: https://github.com/notwa/minisat/tree/glucose-2.0
[glu21]: https://github.com/notwa/minisat/tree/glucose-2.1
[glu30]: https://github.com/notwa/minisat/tree/glucose-3.0
[glu40]: https://github.com/notwa/minisat/tree/glucose-4.0
[glu41]: https://github.com/notwa/minisat/tree/glucose-4.1

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

* MiniSat derivatives will surely make an appearance in
  [the upcoming (July) SAT Race of 2019.][race2019]

* and many more from the [various competitions and races][satcomp]
  held in the past and to be held in the future.

[solvers2016]: https://baldur.iti.kit.edu/sat-competition-2016/solvers/
[solvers2017]: https://baldur.iti.kit.edu/sat-competition-2017/solvers/
[solvers2018]: http://sat2018.forsyte.tuwien.ac.at/solvers/
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
