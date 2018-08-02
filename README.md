About r-jsonlite
================

Home: http://arxiv.org/abs/1403.2805, https://www.opencpu.org/posts/jsonlite-a-smarter-json-encoder

Package license: MIT

Feedstock license: BSD 3-Clause

Summary: A fast JSON parser and generator optimized for statistical data and the web. Started out as a fork of 'RJSONIO', but has been completely rewritten in recent versions. The package offers flexible, robust, high performance tools for working with JSON in R and is particularly powerful for building pipelines and interacting with a web API. The implementation is based on the mapping described in the vignette (Ooms, 2014). In addition to converting JSON data from/to R objects, 'jsonlite' contains functions to stream, validate, and prettify JSON data. The unit tests included with the package verify that all edge cases are encoded and decoded consistently for use with dynamic data in systems and applications.



Current build status
====================

[![Linux](https://img.shields.io/circleci/project/github/conda-forge/r-jsonlite-feedstock/master.svg?label=Linux)](https://circleci.com/gh/conda-forge/r-jsonlite-feedstock)
[![OSX](https://img.shields.io/travis/conda-forge/r-jsonlite-feedstock/master.svg?label=macOS)](https://travis-ci.org/conda-forge/r-jsonlite-feedstock)
[![Windows](https://img.shields.io/appveyor/ci/conda-forge/r-jsonlite-feedstock/master.svg?label=Windows)](https://ci.appveyor.com/project/conda-forge/r-jsonlite-feedstock/branch/master)

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-r--jsonlite-green.svg)](https://anaconda.org/conda-forge/r-jsonlite) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/r-jsonlite.svg)](https://anaconda.org/conda-forge/r-jsonlite) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/r-jsonlite.svg)](https://anaconda.org/conda-forge/r-jsonlite) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/r-jsonlite.svg)](https://anaconda.org/conda-forge/r-jsonlite) |

Installing r-jsonlite
=====================

Installing `r-jsonlite` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
```

Once the `conda-forge` channel has been enabled, `r-jsonlite` can be installed with:

```
conda install r-jsonlite
```

It is possible to list all of the versions of `r-jsonlite` available on your platform with:

```
conda search r-jsonlite --channel conda-forge
```


About conda-forge
=================

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[CircleCI](https://circleci.com/), [AppVeyor](http://www.appveyor.com/)
and [TravisCI](https://travis-ci.org/) it is possible to build and upload installable
packages to the [conda-forge](https://anaconda.org/conda-forge)
[Anaconda-Cloud](http://docs.anaconda.org/) channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](http://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating r-jsonlite-feedstock
=============================

If you would like to improve the r-jsonlite recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/r-jsonlite-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](http://conda.pydata.org/docs/building/meta-yaml.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](http://conda.pydata.org/docs/building/meta-yaml.html#build-number-and-string)
   back to 0.