# QuTiP 2022 Annual Report

Dear QuTiP community,

This last year has again been very productive and successful for QuTiP.

In addition to the usual releases and bug fixes, there has been a big increase
in community events and engagement with QuTiP being showcased at both SciPy and
ASQSQIS, continued fruitful participation in Google Summer of Code and
UnitaryHACK, and a revamp of the QuTiP tutorials which are many users primary
resource when learning QuTiP.

Pleasingly, 2022 has seen a large increase in the number of downloads of QuTiP,
with both the `qutip` and `qutip_qip` packages more than doubling their total
number of downloads.

The end of the year saw the release of **QuTiP 5 alpha**. This a massive
milestone for the community and represents three years of work by members of the
admin team and numerous contributors.

We've summarized the year below, providing short descriptions, links and
statistics where possible.

Thank you again to everyone who contributed this year -- whether by writing
code, filing bug reports, asking or answering questions on the mailing list or
simply using QuTiP. You are all part of our community and much appreciated.

Best wishes and happy quantuming,

The QuTiP Admin Team

## Contents

- [Community Events & Projects](#community-events-and-projects)
- [Downloads and Use](#downloads-and-use)
- [Institutional Support](#institutional-support)
- [Papers](#papers)
- [Major improvements](#major-improvements)
- [Development](#development)
- [Upcoming Projects & Ideas for the Future](#upcoming-projects-ideas-for-the-future)

## Community Events and Projects

- Alex Pitchford and Simon Cross gave a week long QuTiP tutorial at the [African Summer School on Quantum Simulation and Quantum Information](https://indico.ictp.it/event/9807/) in Kigali, Rwanda ([website](https://hodgestar.github.io/qutip-asqsqis-2022/intro.html); [repository](https://github.com/hodgestar/qutip-asqsqis-2022))

- Simon Cross gave a QuTiP tutorial at [SciPy 2022](https://www.scipy2022.scipy.org/) in Austin, Texas ([website](https://hodgestar.github.io/qutip-scipy-2022/intro.html); [repository](https://github.com/hodgestar/qutip-scipy-2022); [video](https://www.youtube.com/watch?v=cUm8lD4btIQ))

- QuTiP GSoC 2022 projects:

    - Christian Staufenbiel ([blog posts](https://christian512.github.io/); QuTiP Tutorials Revamp)
    - Xavier Spronken ([blog posts](https://xspronken.github.io/); Continuous Benchmarks for QuTiP)
    - Shreyas Pradhan ([blog posts](https://medium.com/@claretgrace0801); QuTiP QIP Qiskit Backend)

- QuTiP GSoC 2022 student presentations on the Unitary Fund Discord ([recording](https://www.youtube.com/watch?v=cCzohbNxweM))

- Simon Cross gave a presentation on the HEOM and simulating dynamical decoupling from an environment at AQT in Innsbruck, Austria.

## Downloads and Use

### PyPI downloads

| Package                       | 2021    | 2022    | Growth     |
| :---------------------------- | :-----: | :-----: | :--------: |
| **QuTiP**                     |         |         |            |
| - Downloads (total, all time) | 277 046 | 654 590 | **2.37x**  |
| - Downloads (last 30 days)    | 14 628  | 36 748  | 2.51x      |
| - Dependent packages          | 26      | 39      | 1.50x      |
| **QuTiP QIP**                 |         |         |            |
| - Downloads (total, all time) | 3298    | 13 025  | **3.95x**  |
| - Downloads (last 30 days)    | 509     | 727     | 1.42x      |

Sources:

- [QuTiP @ pepy](https://pepy.tech/project/qutip)
- [QuTiP QIP @ pepy](https://pepy.tech/project/qutip-qip)
- [QuTiP @ libraries.io](https://libraries.io/pypi/qutip/dependents)

### Conda downloads

| Package                       | 2021    | 2022    | Growth     |
| :---------------------------- | :-----: | :-----: | :--------: |
| **QuTiP**                     |         |         |            |
| - Downloads (total, all time) | 407 145 | 502 775 | **1.23x**  |
| - Downloads (last 30 days)    | 5 621   | 4 990   | 0.89x      |

Sources:

- Monthly statistics were collected by running ``condastats overall --monthly qutip``.
- Note: The results returned by ``condastats`` are only from March 2017 onwards. There were an additional 204526 downloads from Anaconda or conda-forge before this. These additional downloads have been added to the overall total to present an accurate picture of the complete history. The full total was obtained from the [Anacoda stats page for QuTiP](https://anaconda.org/conda-forge/qutip).

### Mailing list

- [350 threads in 2022](https://groups.google.com/g/qutip/search?q=after%3A2022-01-01%20before%3A2022-12-31) (vs 255 last year)

## Institutional Support

### RIKEN

- Simon Cross worked on QuTiP full-time at RIKEN this year, funded via the Moonshot grant program.

### Unitary Fund

- QuTiP is supported by Unitary Fund as an affiliated project.

- The QuTiP community calls are being held on the Unitary Fund Discord.

- QuTiP was one of the featured projects in [UnitaryHACK 2022](https://unitaryhack.dev/projects/qutip/), a distributed bounty hack supporting quantum open source software. Three hacks were awarded (see GitHub issues [\#1526](https://github.com/qutip/qutip/issues/1526), [\#1893](https://github.com/qutip/qutip/issues/1893), [\#1894](https://github.com/qutip/qutip/issues/1894)).

The two Unitary Fund grants awarded last year were completed and merged into QuTiP and QuTiP QIP respectively this year:

- Diego Wiskniacki and his students' PyKrylovSolver ([blog post](https://unitary.fund/posts/krylov.html)) was merged into QuTiP on 8 April 2022 in [https://github.com/qutip/qutip/pull/1739].

- Ben Braham's Variational Quantum Algorithms and quantum optimal control project (supervised by Daniel Burgarth) was merged into QuTiP QIP on 22 April 2022 in [https://github.com/qutip/qutip-qip/pull/123/]. It is available as `qutip_qip.vqa`.

### NumFOCUS

- QuTiP remains a NumFOCUS [affiliated project](https://numfocus.org/sponsored-projects/affiliated-projects).

- In 2022, QuTiP took part in Google Summer of Code under the NumFOCUS umbrella.

## Papers

- *"Pulse-level noisy quantum circuits with QuTiP"* by Boxi Li, Shahnawaz Ahmed, Sidhant Saraogi, Neill Lambert, Franco Nori, Alexander Pitchford, Nathan Shammah, *[Quantum](https://quantum-journal.org/papers/q-2022-01-24-630/)* **6**, 630 (2022).

- *"QuTiP-BoFiN: A bosonic and fermionic numerical hierarchical-equations-of-motion library with applications in light-harvesting, quantum control, and single-molecule electronics"* by Neill Lambert, Tarun Raheja, Simon Cross, Paul Menczel, Shahnawaz Ahmed, Alexander Pitchford,Daniel Burgarth, Franco Nori, *[arxiv.org](https://arxiv.org/abs/2010.10806)* (2023). Submitted for publication.

- [21 arxiv.org papers references QuTiP](https://arxiv.org/search/?query=qutip&searchtype=all&source=header)

## Major improvements

- QuTiP 5.0.0a1 released.

- The tutorials were updated to support both QuTiP 5 and QuTiP 4.7, and are now tested nightly to ensure they don't become outdated in the future.

- Nightly benchmarks were implemented for the QuTiP 5 data layer and solvers.

- The remaining solvers were ported to the new QuTiP 5 solver interface, including the Monte-Carlo, Bloch-Redfield, Kyrlov Subspace, Floquet, HEOM, and Evolution of State solvers. Related functionality including the calculation of propagators, steady states and correlation functions were also migrated.

- Integration tests for Windows were activated and Windows is now a fully supported platform.

- Support for Apple M1 was added and binaries packages for the Apple M1 are available from conda-forge.

- QuTiP was compiled for Web Assembly and can be run natively inside a browser. A compiled package is available from emscripten-forge.

- Support has been added for 64-bit integer sparse matrix indices.

- The Krylov subspace and Hierarchical Equations of Motion (HEOM) solvers were released.

## Development

- QuTiP releases:

    - [4.6.3](https://github.com/qutip/qutip/releases/tag/v4.6.3) (9 February 2022)

    - [4.7.0](https://github.com/qutip/qutip/releases/tag/v4.7.0) (13 April 2022)

    - [4.7.1](https://github.com/qutip/qutip/releases/tag/v4.7.1) (12 December 2022)

    - [5.0.0a1](https://github.com/qutip/qutip/releases/tag/v5.0.0a1) (8 February 2023)

- QuTiP QIP releases:

    - [0.2.1](https://github.com/qutip/qutip-qip/releases/tag/v0.2.1) (20 February 2022)

    - [0.2.2](https://github.com/qutip/qutip-qip/releases/tag/v0.2.2) (19 June 2022)

    - [0.2.3](https://github.com/qutip/qutip-qip/releases/tag/v0.2.3) (12 December 2022)

- QuTiP commits:

    - 35 people made commits to the main QuTiP repository (45 last year)

    - 11 people made more than 10 commits each (16 last year)

    - 1174 commits in total (902 last year)

- QuTiP issues:

    - [97 issues created](https://github.com/qutip/qutip/issues?q=is%3Aissue+is%3Aopen+created%3A2022-01-01..2022-12-31) (of which 70 have been resolved; vs 108 created last year)
    - [102 issues closed](https://github.com/qutip/qutip/issues?q=is%3Aissue+is%3Aopen+closed%3A2022-01-01..2022-12-31) (vs 151 closed last year)
    - [163 issues updated](https://github.com/qutip/qutip/issues?q=is%3Aissue+is%3Aopen+updated%3A2022-01-01..2022-12-31) (of which 103 have been resolved; vs 217 updated last year)
    - Currently open: 132 (vs 134 last year)

- QuTiP pull requests:

    - [206 pull requests created](https://github.com/qutip/qutip/pulls?q=is%3Apr+is%3Aopen+created%3A2022-01-01..2022-12-31) (of which 199 have been closed; vs 194 created last year)
    - [215 pull requests closed](https://github.com/qutip/qutip/pulls?q=is%3Apr+is%3Aopen+closed%3A2022-01-01..2022-12-31) (vs 199 closed last year)
    - [271 pull requests updated](https://github.com/qutip/qutip/pulls?q=is%3Apr+is%3Aopen+updated%3A2022-01-01..2022-12-31) (of which 263 have been closed; vs 317 updated last year)
    - [180 pull requests merged](https://github.com/qutip/qutip/pulls?q=is%3Apr+is%3Aopen+merged%3A2022-01-01..2022-12-31) (vs 160 merged last year)
    - Currently open: 13

- A new data layer was created (as part of a TU Delft MSc internship):

    - [TensorNetwork backend](https://github.com/qutip/qutip-tensornetwork/) (by [Asier Galicia](https://github.com/AGaliciaMartinez))

- A new benchmark suite for QuTiP 5 was implemented (as part of GSoC):

    - [website](https://qutip.org/qutip-benchmark/)
    - [qutip-benchmark](github.com/qutip/qutip-benchmark/)
    - by [Xavier Spronken](https://github.com/xspronken)

- The QuTiP tutorials underwent a major overhaul in order to support QuTiP 5 and
  4 and to ensure that they are continually tested from now onwards (as part
  of GSoC):

    - [website](https://qutip.org/qutip-tutorials/)
    - [qutip-tutorials](https://github.com/qutip/qutip-tutorials)
    - by [Christian Staufenbiel](https://github.com/christian512)
    - the [qutip-notebooks](https://github.com/qutip/qutip-notebooks) repository is now deprecated.

- QuTiP was compiled for WebAssembly and can now be run entirely in a browser:

    - [emscriptem-forge recipe](https://github.com/emscripten-forge/recipes/tree/main/recipes/recipes_emscripten/qutip) (builds the emscriptem-forge package)
    - [emscriptem-forge package](https://beta.mamba.pm/channels/emscripten-forge/packages/qutip)
    - [try-qutip](https://github.com/qutip/try-qutip/) (JupyterLite configuration)
    - [website](http://qutip.org/try-qutip/)

## Upcoming Projects & Ideas for the Future

- We expect 4.7.2 and 5.0.0 to be released in the first half of 2023.

- We expect QuTiP 5 to undergo a period of stabilization, bug fixing and polishing as more people start using it.

- We expect `qutip.control` to be moved to its own family package before the 5.0.0 release.

- We expect QuTiP 4.7 to be maintained indefinitely in order to allow users to transition to QuTiP 5.

- QuTiP are participating in Google Summer of Code 2023 with NumFOCUS ([project ideas](https://github.com/qutip/qutip/wiki/Google-Summer-of-Code-2023)).
