README
================

[![Build Status](https://travis-ci.org/lorenzwalthert/strcode.svg?branch=master)](https://travis-ci.org/lorenzwalthert/strcode) [![Project Status: WIP ? Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](http://www.repostatus.org/badges/latest/wip.svg)](http://www.repostatus.org/#wip) [![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/strcode)](https://cran.r-project.org/package=strcode) [![packageversion](https://img.shields.io/badge/Package%20version-0.2.0-orange.svg?style=flat-square)](commits/master)

# Table of Contents
1. Introduction
2. Installation
3. Adding YesWorkflow annotations in R scripts
4. Generating RDF from YesWorkflow annotations

<a id="intro"></a>
# Introduction


This special version of the `strcode` package (short for "structuring code") contains tools to help you organize and abstract your R scripts and to embed semantics according to the [ProvONE Data Model for Workflow Semantics](http://bit.ly/2eOUuAX). It consists of:
- An [RStudio Add-in](https://rstudio.github.io/rstudioaddins/) that lets you quickly insert code block separators and titles (possibly with unique identifiers) to divide your work into sections. The titles are recognized as sections by RStudio, which further enhances the coding experience.
- A function `sum_str` that summarizes the code structure based on the separators and comments added with the Add-in. For one or more files, it can send the structure to the console or a file. 
  - **NEW**: The `sum_str` function now can structure code with **embedded semantics** and can generate RDF files (N3 format) 
`sum_str` has built-in rules for automatic property generation for `ProvONE` entity types.
- An [RStudio Add-in](https://rstudio.github.io/rstudioaddins/) that lets you insert a code anchor, that is, a hash sequence which can be used to uniquely identify a line in a large code base.

<!-- You can learn more about structuring code in [Bono Usu](https://github.com/lorenzwalthert/bonousu/blob/devel/docs/commenting-code.html), 
a guide for good practice in R programming. -->



<a id="install"></a>
# Installation

You can install the package from GitHub.

``` r
# install.packages("devtools")
devtools::install_github("IndependentStudy2017YW")
```
<a id="structuring"></a>

# Adding YesWorkflow annotations in R scripts
The animation below shows using `strcode` for embedding YesWorkflow annotations in R scripts. 

<img src="https://github.com/XiaoliangJiang/IndependentStudy2017YW/blob/master/demos/Generating%20YesWorkflow%20Annotations.gif" width="800px" />



# Generating RDF from YesWorkflow annotations
