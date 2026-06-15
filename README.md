
# aeaegypticdmx

<!-- badges: start -->
<!-- badges: end -->

**aegypticdmx** is an R package (version 0.1.0) that provides data on the presence of *Ae. aegypti* in the Mexico City metropolitan area, along with machine learning algorithms to predict its presence. It was developed and is maintained by Felipe Antonio Dzul Manzanilla (ORCID: 0000-0002-2085-9141), and is released under the MIT license.

## Installation

You can install the development version of aeaegypticdmx from [GitHub](https://github.com/) with:

``` r
# install.packages("pak")
pak::pak("fdzul/aeaegypticdmx")
```

## Datasets 

- ae_aegypti_cdmx is an sf object with 214 rows and 43 variables that contains records of the presence/pseudo-absence of Ae. aegypti in the urban area of the Mexico City metropolitan zone. Details of the variables can be found at [zenodo](https://zenodo.org/records/20708053) or via the code *?aeaegypticdmx::ae_aegypti_cdmx* or *Reference*.

- aoi. The study area. It is an sf object with the delimitation of the global urban area of Mexico City, obtained from the Facebook/Meta Global Urban Areas product (Data for Good).


## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(aeaegypticdmx)
gtExtras::gt_plt_summary( aeaegypticdmx::ae_aegypti_cdmx|> sf::st_drop_geometry())
```

## Articles 

In the *Articles* section, you will find the reproducible code for predicting the presence of *Ae. aegypti* in the Mexico City metropolitan area using LightGBM.

