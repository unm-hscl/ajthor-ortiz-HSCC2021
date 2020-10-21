# ajthor-ortiz-HSCC2021

Code for the paper, "SReachTools Kernel Module: Data-Driven Stochastic Reachability Using Hilbert Space Embeddings of Distributions," HSCC 2021.

The code is provided in a CodeOcean capsule, located [here](https://codeocean.com/capsule/6944595/tree).

## Table of Contents

* [Documentation](#documentation)
* [Instructions](#instructions)
  * [Requirements](#requirements)
  * [Repeatability Instructions](#repeatability-instructions)

## Description

This repository contains the repeatability code and documentation for the
algorithms and plots presented in "SReachTools Kernel Module: Data-Driven
Stochastic Reachability Using Hilbert Space Embeddings of Distributions". It
contains an implementation of two algorithms, called `KernelEmbeddings` and
`KernelEmbeddingsRFF`, included in the upcoming release of
[SReachTools](https://sreachtools.github.io).

## Documentation

Documentation for the code is provided throughout. The documentation is
formatted as easily-readable
[Markdown](https://guides.github.com/features/mastering-markdown/). Each folder
contains a top-level description of the folder contents and the purpose of the
code contained inside, each file also contains comments and documentation to
describe the code purpose and usage. More information and updates can be found
at the [SReachTools website](https://sreachtools.github.io).

## Instructions

* **How do I get the code?**
The code is provided as a CodeOcean capsule, located
[here](https://codeocean.com/capsule/6944595/tree). Alternatively, the code can
be downloaded by
[exporting](https://help.codeocean.com/en/articles/2199842-exporting-capsules-and-reproducing-results-on-your-local-machine)
the CodeOcean capsule to your system, with repeatability instructions provided
in the `REPRODUCING.md` file generated by CodeOcean. The code can also be cloned
using [git](https://git-scm.com) from the GitHub repository page
[ajthor-ortiz-HSCC2021](https://github.com/unm-hscl/ajthor-ortiz-HSCC2021) using
the following command, or downloaded directly using the following link:
https://github.com/unm-hscl/ajthor-CDC2020/archive/master.zip
```shell
git clone https://github.com/unm-hscl/ajthor-ortiz-HSCC2021.git
```
Use the [Dockerfile](environment/Dockerfile) to build the Docker image, and run
the code from within the container. This will require you to attach a Matlab
license to the container, and is recommended only for advanced users.
* **How do I use the code?**
It is recommended that the code be run from the CodeOcean capsule, located
[here](https://codeocean.com/capsule/6944595/tree), using the 'Reproducible Run'
button.
* **I just want to see the implementation.**
Implementations of the algorithms are located [here](code/implementations/).

### Requirements

This code has been tested and run on macOS 10.14.6 (Mojave), as well as Ubuntu
18.04.3 (Bionic Beaver) using Matlab 9.6.0.1174912 (R2019a) Update 5. It should
also run in any newer version of Matlab.

* **Does the code have any dependencies?**
The `KernelEmbeddings` and `KernelEmbeddingsRFF` algorithms require
[SReachTools](https://sreachtools.github.io) to be downloaded and installed on
your system, but has no additional dependencies. Other algorithms in
[SReachTools](https://sreachtools.github.io) require [MPT](https://www.mpt3.org)
and [CVX](http://cvxr.com), and may also require a solver such as
[Gurobi](https://www.gurobi.com).

### Repeatability Instructions

It is recommended that the code be run from the CodeOcean capsule, located
[here](https://codeocean.com/capsule/6944595/tree). On the capsule page, click
'Reproducible Run' to run the code and generate all figures.

If you would like to reproduce the results locally, download the CodeOcean
capsule by
[exporting](https://help.codeocean.com/en/articles/2199842-exporting-capsules-and-reproducing-results-on-your-local-machine)
the CodeOcean capsule to your system and following the instructions in the
`REPRODUCING.md` file generated by CodeOcean. 

The main entry points for the code are located in the `code` directory and are
labeled `run.sh` and `run_all.m`. These scripts generate the figures and tables
used in the paper and should serve as the main repeatability files.
