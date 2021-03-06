
<!-- README.md is generated from README.Rmd. Please edit that file -->

# neotomaTargets

`neotomaTargets` is a template for reproducible research using data from
the [Neotoma database](https://www.neotomadb.org/) using the
[`targets`](https://books.ropensci.org/targets/) pipeline.

It includes sample code for downloading data from Neotoma, cleaning the
data, analysing the data, and writing a manuscript with R markdown, all
in a `targets` pipeline.

The aim is that you can make a copy of the template and modify it to
write your own reproducible manuscripts.

# Installation

`neotomaTargets` is a [template
repository](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/creating-a-repository-from-a-template).

Click on the :green\_square: `Use this template` :green\_square: button
and follow the instructions to make a copy of this repo into your own
account.

`neotomaTargets` depends on the `neotoma` and `targets` packages and
some others listed in the DESCRIPTION file. To install these packages,
use

``` r
devtools::install_deps()
```

# Using neotomaTemplate

To run all the analyses and produce the manuscript, open “make.R” and
run `tar_make()`. This finds the target plan in "\_targets.R" (this file
must have this name and be in the working directory), which is assembled
from sub-plans in "R/\*-plan.R" files. If you modify any of the
sub-plans and re-run `tar_make()` only targets which have been outdated
will be re-run.
