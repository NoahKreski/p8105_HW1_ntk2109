p8105\_HW1\_ntk2109\_markdown
================
Noah Kreski

Problem 1 - Creating a data frame comprised of:

A random sample of size 10 from a uniform \[0,5\] distribution

A logical vector indicating whether elements of the sample are greater than 2

A (length-10) character vector

A (length-10) factor vector

``` r
set.seed(1)

question_one_df = tibble(
  uniform_samp = runif(10, 0, 5),
  logical_vec_one = c((uniform_samp)>2),
  character_vec_one = c("This", "is", "a", "character", "vector", "that", "has", "length", "of", "ten"),
  factor_vec_one = c("male", "female","male", "female","male", "female","male", "female","male", "female")
)
```

2.7575694 0.6 NA NA
