# MiniSat etc.

This repository contains various forks and patches of MiniSat
written by various authors over the years.
[The original MiniSat][homepage] is written and
Copyright ⓒ 2003-2006 Niklas Eén, Copyright ⓒ 2003-2010 Niklas Sörensson,
and distributed under the terms of [the MIT license.][license_mit]

In the [master branch,][master] a version based on [Niklas's most recent work][upstream]
is patched and ready to compile with modern compilers.

In the [patches branch,][patches] various patch files have been archived.

In the [COMiniSatPS branch,][comsps] Chanseok Oh's patches have been applied
to version 2.2.0. [Visit the COMiniSatPS homepage. (archived)][comsps_archive]

The ubiquitous [version 2.2.0 is available here,][v220]
and the earlier [version 2.0 is available here.][v200]
Earlier than that, a few select versions
are available on [the MiniSat homepage.][homepage]

You can download any of the versions on GitHub by following the appropriate link
and clicking on the green "Clone or download" link on the top right.
Select "Download Zip" if you're not familiar with git.

[homepage]: http://minisat.se/MiniSat.html
[master]: https://github.com/notwa/minisat/tree/master
[upstream]: https://github.com/niklasso/minisat/tree/master
[patches]: https://github.com/notwa/minisat/tree/patches
[comsps]: https://github.com/notwa/minisat/tree/COMiniSatPS
[comsps_archive]: https://web.archive.org/web/20171023151341/http://www.cs.nyu.edu/~chanseok/cominisatps/
[license_mit]: https://choosealicense.com/licenses/mit/
[v220]: https://github.com/notwa/minisat/tree/releases/2.2.0
[v200]: https://github.com/notwa/minisat/tree/releases/2.0.0

## Other Versions

These versions have been omitted from this repository
because they are already readily accessible.

### CryptoMiniSat

[CryptoMiniSat][cms] is a major rewrite of MiniSat, adding many features,
including XOR clauses for improved solving of cryptographic problems.
CryptoMiniSat is written and maintained by [Mate Soos](https://www.msoos.org/)
on [the CryptoMiniSat GitHub repository.][cms]

[cms]: https://github.com/msoos/cryptominisat

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
