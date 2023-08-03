
<!-- README.md is generated from README.Rmd. Please edit that file -->

# libminer

<!-- badges: start -->
<!-- badges: end -->

The goal of libminer is to provide an overview of your R library setup.
It is a toy package created as a part of a workshop and not meant for
serious use.

## Installation

You can install the development version of libminer from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("ateucher/libminer")
```

## Example usage

To get a count of installed packages in each of your library locations,
optionally with the total sizes, use the `lib_summary()` function:

``` r
library(libminer)
lib_summary()
#>                                                                                         Library
#> 1                          /Library/Frameworks/R.framework/Versions/4.3-arm64/Resources/library
#> 2 /private/var/folders/_f/n9fw7ctx3fqf2ty9ylw502g80000gn/T/RtmpTxIv1Z/temp_libpath17e816c6e95f9
#> 3                                                       /Users/andy/Library/R/arm64/4.3/library
#>   n_packages
#> 1         29
#> 2          1
#> 3        191
# specify `sizes = TRUE` to calculate the total size on disk of your packages
lib_summary(sizes = TRUE)
#>                                                                                         Library
#> 1                          /Library/Frameworks/R.framework/Versions/4.3-arm64/Resources/library
#> 2 /private/var/folders/_f/n9fw7ctx3fqf2ty9ylw502g80000gn/T/RtmpTxIv1Z/temp_libpath17e816c6e95f9
#> 3                                                       /Users/andy/Library/R/arm64/4.3/library
#>   n_packages   lib_size
#> 1         29   71351828
#> 2          1      14402
#> 3        191 1164955163
```
