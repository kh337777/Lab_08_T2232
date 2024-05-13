DSC 200 Lab08 - Importing Data -Term 2232
================
2024-05-13

**Student Name:<Khulud>**

**Student ID:\<2221004941\>**

## Loading Packages

``` r
library(tidyverse)
```

## Tasks

\`1. Read in the nobels.csv file from the data/ folder.

``` r
nobel <- read_csv(file = "data/nobel.csv")
```

    ## Rows: 935 Columns: 26
    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr  (21): firstname, surname, category, affiliation, city, country, gender,...
    ## dbl   (3): id, year, share
    ## date  (2): born_date, died_date
    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

``` r
nobel
```

    ## # A tibble: 935 × 26
    ##       id firstname   surname  year category affiliation city  country born_date 
    ##    <dbl> <chr>       <chr>   <dbl> <chr>    <chr>       <chr> <chr>   <date>    
    ##  1     1 Wilhelm Co… Röntgen  1901 Physics  Munich Uni… Muni… Germany 1845-03-27
    ##  2     2 Hendrik A.  Lorentz  1902 Physics  Leiden Uni… Leid… Nether… 1853-07-18
    ##  3     3 Pieter      Zeeman   1902 Physics  Amsterdam … Amst… Nether… 1865-05-25
    ##  4     4 Henri       Becque…  1903 Physics  École Poly… Paris France  1852-12-15
    ##  5     5 Pierre      Curie    1903 Physics  École muni… Paris France  1859-05-15
    ##  6     6 Marie       Curie    1903 Physics  <NA>        <NA>  <NA>    1867-11-07
    ##  7     6 Marie       Curie    1911 Chemist… Sorbonne U… Paris France  1867-11-07
    ##  8     8 Lord        Raylei…  1904 Physics  Royal Inst… Lond… United… 1842-11-12
    ##  9     9 Philipp     Lenard   1905 Physics  Kiel Unive… Kiel  Germany 1862-06-07
    ## 10    10 J.J.        Thomson  1906 Physics  University… Camb… United… 1856-12-18
    ## # ℹ 925 more rows
    ## # ℹ 17 more variables: died_date <date>, gender <chr>, born_city <chr>,
    ## #   born_country <chr>, born_country_code <chr>, died_city <chr>,
    ## #   died_country <chr>, died_country_code <chr>, overall_motivation <chr>,
    ## #   share <dbl>, motivation <chr>, born_country_original <chr>,
    ## #   born_city_original <chr>, died_country_original <chr>,
    ## #   died_city_original <chr>, city_original <chr>, country_original <chr>

Write your narrative here

\`2. Split into two (STEM and non-STEM)

\`2.1. Create a new data frame, nobel_stem, that filters for the STEM
fields (Physics, Medicine, Chemistry, and Economics).

Write your narrative below

\`2.2. Create another data frame, nobel_nonstem, that filters for the
remaining fields.

Write your narrative here

\`3. Write out the two data frames to nobel-stem.csv and
nobel-nonstem.csv, respectively, to data/.

Write your narrative here

\`4. Load the sales.xlsx file from the data/ folder, using appropriate
arguments for the read_excel() function such that it looks like the
output on the left (see lab handout).

Write your narrative here

\`5. Manipulate the sales data to look like the output on the right (see
lab handout).

Write your narrative here

\`6. Write out the manipulated data frame to data/sales_last.xlsx to
folder.

Write your narrative here
