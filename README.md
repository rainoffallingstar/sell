
<!-- README.md is generated from README.Rmd. Please edit that file -->

# sell
<img src="https://github.com/rainoffallingstar/sell/blob/master/dev/sell.png" height="200" align="right"/>
<!-- badges: start -->
<!-- badges: end -->

The goal of sell is to build a R6-based package for singlecell analysis. Now warped with Seurat V4/V5.

## Installation

You can install the development version of sell like so:

``` r
# FILL THIS IN! HOW CAN PEOPLE INSTALL YOUR DEV PACKAGE?
pak::pak("rainoffallingstar/sell")
```

## Example

This is a basic example which shows you how to solve a common problem:

```{r example}
library(sell)
## basic example code
## check seurat api
seurat_api_detect()

## encode your array and pdata into seurat object and take computation
seurat_object <- seurat_encoder(newdata[["arraydata"]],newdata[["pdata"]],min.cells = 0,
                           min.features = 0,reduction_dims = 1:5)
## extract datas from seurat container

sell_list <- seurat_decoder(seurat_object)

```
