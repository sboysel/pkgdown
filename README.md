
<!-- README.md is generated from README.Rmd. Please edit that file -->
pkgdown
=======

[![Travis-CI Build Status](https://travis-ci.org/hadley/pkgdown.svg?branch=master)](https://travis-ci.org/hadley/pkgdown) [![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/pkgdown)](https://cran.r-project.org/package=pkgdown) [![Coverage Status](https://img.shields.io/codecov/c/github/hadley/pkgdown/master.svg)](https://codecov.io/github/hadley/pkgdown?branch=master)

pkgdown is designed to make it quick and easy to build a website for your package. You can see pkgdown in action at <http://hadley.github.io/pkgdown/>: this is the output of pkgdown applied to the latest version of pkgdown. Learn more in `vignette("pkgdown")` or `?build_site`.

Installation
------------

pkgdown is not currently available from CRAN, but you can install the development version from github with:

``` r
# install.packages("devtools")
devtools::install_github("hadley/pkgdown")
```

Usage
-----

Run pkgdown from the package directory each time you release your package:

``` r
pkgdown::build_site()
```

This will generate a `docs/` directory. The home page will be generated from your package's `README.md`, and a function reference will be generated from the documentation in the `man/` directory. If you are using GitHub, the easiest way to make this your package website is to check into git, then go settings for your repo and make sure that the **GitHub pages** source is set to "master branch /docs folder".

The package also includes an RStudio add-in which you can bind to a keyboard shortcut. I recommend `Cmd + Shift + W`: it uses Cmd + Shift, like all other package development worksheets, it replaces a rarely used command (close all tabs), and the W is mnemonic for website.

To customise your site, create `_pkgdown.yml` and modify it as described in the documentation. Alternatively, you can also use `pkgdown/_pkgdown.yml` if you need other files to customise your site.
