# QuTiP 2021 Annual Report

Dear QuTiP community,

The QuTiP Admin Team is happy to report that 2021 has been a busy,
productive and successful year for QuTiP with many new features, bugs
fixed, and contributions from the community.

We've summarized these below, providing short descriptions and links and
statistics where possible.

This year was also **QuTiP's 10th anniversary** -- congratulations and
thank you's to everyone who contributed to getting us where we are
today, and here's to the next ten years!

**Asier Galicia has been welcomed to the QuTiP admin team**.

[QuTiP 2021 Annual Report](#qutip-2021-annual-report)

[Community Events & Projects](#community-events-and-projects)

[Downloads and Use](#downloads-and-use)
[Unitary Fund Grants to QuTiP projects](#unitary-fund-support)
[Jobs](#jobs)
[Papers](#papers)
[Major improvements](#major-improvements)
[Development](#development)
[Upcoming Projects & Ideas for the Future](#upcoming-projects-ideas-for-the-future)

## Community Events and Projects

-   QuTiP's [10-year anniversary](https://unitary.fund/posts/qutip_10_years.html) on Unitary Fund's Discord server

-   QuTiP GSoC 2021 projects:

    -   Felipe Haiek ([blog posts](https://felipebihaiek.medium.com/); CuPy data backend)

    -   Purva Thakre ([blog posts](https://purva-thakre.github.io/purva-blog/); converting unitaries to gates)

    -   Asier Galicia ([blog posts](https://agalicia.netlify.app/tag/gsoc/); TensorFlow data backend)

-   QuTiP GSoC + QuTiP 5 community call on Unitary Fund Discord:

    -   [A CuPy backend for QuTiP](https://www.youtube.com/watch?v=e4dvd7_kRXQ) (Felipe Haiek)

    -   [qutip-tensorflow](https://www.youtube.com/watch?v=UPYIlapJaMQ) (Asier Galicia)

    -   [Quantum Gate Decomposition](https://www.youtube.com/watch?v=3iP4mimbIzs) (Purva Thakre)

    -   [QuTiP 5 Status](https://www.youtube.com/watch?v=u2LubstAgqY) (Simon Cross)

-   Asier Galicia joined the QuTiP admin team in December for his TUDelft MSc internship to work on a TensorNetwork data backend ([qutip-tensornetwork](https://github.com/qutip/qutip-tensornetwork/))

-   Four students from the Maastricht Science Program produced a tutorial on [Single Photon Interference](https://nbviewer.ipython.org/github/qutip/qutip-notebooks/blob/master/examples/single-photon-interference-example.ipynb) as part of a four week project in June.

-   QuTiP QIP mini-meetup in Cologne was attended by Boxi, Simon &  Gaurav Saxena

-   QuTiP participated in Nvidia's cuQuantum beta release program and gave feedback (Simon, Neill, Asier)

-   QuTiP Admins helped CINECA (Italy's supercomputing facility) understand how to accelerate QuTiP by high performance computing (HPC). [Link](https://github.com/qutip/qutip/issues/1671) to issue.

## Downloads and Use

-   Total downloads from PyPI (and last 30 days):

    -   QuTiP: [277 046](https://pepy.tech/project/qutip)(14 628)

    -   QuTiP QIP: [3298](https://pepy.tech/project/qutip-qip) (509)

-   Packages that depend on QuTiP: [26](https://libraries.io/pypi/qutip/dependents)

## Unitary Fund Support

-   QuTiP is supported by Unitary Fund as an affiliated project.

-   The QuTiP community calls are being held on the Unitary Fund Discord.

```{=html}
<!-- -->
```
-   QuTiP was one of the featured projects in [UnitaryHACK](https://unitaryfund.github.io/unitaryhack/participating-projects.html#qutip), a distributed bounty hack supporting quantum open source software. Three hacks were awarded.

Unitary Fund has awarded the following grants for projects involving
QuTiP:

-   To Diego Wiskniacki and his students to build PyKrylovSolver ([blog post](https://unitary.fund/posts/krylov.html), opened PR [\#1739](https://github.com/qutip/qutip/pull/1739))

-   To Ben Braham for an undergoing project on Variational Quantum Algorithms + quantum optimal control (supervised by Daniel Burgarth). An issue ([\#118](https://github.com/qutip/qutip-qip/issues/118)) has been opened on qutip-qip

## Jobs

-   Added Asier Galicia (former GSoC student and RIKEN intern) to the qutip admins. He is working on qutip-tensornetworks.

-   RIKEN[:]

    -   Simon Cross started full-time at RIKEN in May (focused on QuTiP development)

    -   A second position at RIKEN to work on QuTiP remains open ([job ad](https://qutip.org/jobs.html))

## Papers

-   *"Pulse-level noisy quantum circuits with QuTiP"* by Boxi Li, Shahnawaz Ahmed, Sidhant Saraogi, Neill Lambert, Franco Nori, Alexander Pitchford, Nathan Shammah,[*[Quantum]{.ul}*](https://quantum-journal.org/papers/q-2022-01-24-630/) **6**, 630 (2022).

```{=html}
<!-- -->
```
-   "*BoFiN-HEOM: A bosonic and fermionic numerical hierarchical-equations-of-motion library with applications in light-harvesting, quantum control, and single-molecule electronics*" by Neill Lambert, Tarun Raheja, Simon Cross, Paul Menczel, Shahnawaz Ahmed, Alexander Pitchford,Daniel Burgarth, Franco Nori \[soon to be updated\]

## Major improvements

-   QobjEvo and Coefficients (i.e. support for time-dependent systems) were greatly improved

-   A pluggable system of solvers and ODE integrators was added.

-   State of the art Verner ODE integrators that use the new data layer were added (see [Refuge for Runge-Kutta Pairs](http://people.math.sfu.ca/~jverner/))

-   QuTiP's new data layer was completed

-   QuTiP QIP was split out from QuTiP itself (the first split out family package)

-   The Hierarchy Equations of Motion (HEOM) solver was reimplemented, starting from the BoFiN HEOM ([examples](https://github.com/qutip/qutip-notebooks/blob/762a9ce48f27c0992072b41d709c9bbb9131ab90/examples/heom/heom-index.ipynb)) and a new guide was written for it.

-   To support the qutip-cupy project, GPU test runners were set up on AWS which can be used to test QuTiP projects on GPUs in the future.

-   QuTiP release process was automated and [documented](https://qutip.org/docs/latest/development/release_distribution.html)

-   QuTiP documentation is now built using a GitHub action (previously it was hand build in a hard to reproduce way)

## Development

-   QuTiP releases:

    -   [4.5.3](https://github.com/qutip/qutip/releases/tag/v4.5.3)(19 February 2021)

    -   [4.6.0](https://github.com/qutip/qutip/releases/tag/v4.6.0)(11 April 2021)

    -   [4.6.1](https://github.com/qutip/qutip/releases/tag/v4.6.1)(5 May 2021)

    -   [4.6.2](https://github.com/qutip/qutip/releases/tag/v4.6.2)(2 June 2021)

-   QuTiP QIP releases:

    -   [0.1.0](https://github.com/qutip/qutip-qip/releases/tag/v0.1.0)(14 May 2021)

    -   [0.1.1](https://github.com/qutip/qutip-qip/releases/tag/v0.1.1)(28 July 2021)

    -   [0.1.2](https://github.com/qutip/qutip-qip/releases/tag/v0.1.2)(24 November 2021)

    -   [0.2.0](https://github.com/qutip/qutip-qip/releases/tag/v0.2.0)(26 November 2021)

-   QuTiP commits:

    -   45 people made commits to the main QuTiP repository

    -   16 people made more than 10 commits each

    -   902 commits in total

-   QuTiP issues:

    -   [108 issues created](https://github.com/qutip/qutip/issues?q=is%3Aissue+is%3Aopen+created%3A2021-01-01..2021-12-31)
        > (of which 81 have been resolved)

    -   [151 issues closed](https://github.com/qutip/qutip/issues?q=is%3Aissue+is%3Aopen+closed%3A2021-01-01..2021-12-31+)

    -   [217 issues updated](https://github.com/qutip/qutip/issues?q=is%3Aissue+is%3Aopen+updated%3A2021-01-01..2021-12-31+)

    -   Currently open: 134

-   QuTiP pull requests:

    -   [194 pull requests created](https://github.com/qutip/qutip/pulls?q=is%3Apr+is%3Aopen+created%3A2021-01-01..2021-12-31+)(of which 183 have been closed)

    -   [199 pull requests closed](https://github.com/qutip/qutip/pulls?q=is%3Apr+is%3Aopen+closed%3A2021-01-01..2021-12-31+)

    -   [317 pull requests updated](https://github.com/qutip/qutip/pulls?q=is%3Apr+is%3Aopen+updated%3A2021-01-01..2021-12-31+)

    -   [160 pull requests merged](https://github.com/qutip/qutip/pulls?q=is%3Apr+is%3Aopen+merged%3A2021-01-01..2021-12-31+)

    -   Currently open: 20

-   Two new data layers created (as part of GSoC):

    -   [TensorFlow backend](https://github.com/qutip/qutip-tensorflow/)([Asier Galicia](https://github.com/AGaliciaMartinez))

    -   [CuPy backend](https://github.com/qutip/qutip-cupy/)([Felipe Haiek](https://github.com/MrRobot2211))

## Upcoming Projects & Ideas for the Future

-   We expect QuTiP 4.6.3, QuTiP 4.7 and the alpha release of QuTiP 5 to
    > all take place in Q1/Q2 2022.

-   We then expect a period of some months improving the alpha release
    > and getting community feedback before moving onto a beta release.

-   We expect QuTiP 4.7 to be maintained for some time in order to allow
    > users to transition to QuTiP 5.

-   QuTiP are participating in Google Summer of Code 2022 with NumFOCUS,
    > applications start today, April 4th, 2022 and close April
    > 19th, 2022. Any help in spreading the word is welcome. Here the
    > link to the project ideas, which are:

    -   [1 - QuTiP Notebooks
        > 5](https://github.com/qutip/qutip/wiki/Google-Summer-of-Code-2022#qutip-notebooks-5)

    -   [2 - QuTiP
        > Benchmarks](https://github.com/qutip/qutip/wiki/Google-Summer-of-Code-2022#qutip-benchmarks)

    -   [3 - QuTiP Virtual
        > Lab](https://github.com/qutip/qutip/wiki/Google-Summer-of-Code-2022#qutip-virtual-lab)

    -   [4 - qutip-qip as a Qiskit
        > backend](https://github.com/qutip/qutip/wiki/Google-Summer-of-Code-2022#qutip-qip-as-a-Qiskit-backend)

    -   [5 - JAX data
        > backend](https://github.com/qutip/qutip/wiki/Google-Summer-of-Code-2022#JAX-data-backend)
