p8105\_HW1\_ntk2109\_markdown
================
Noah Kreski

Question One
------------

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
  factor_vec_one = factor(c("male", "female","male", "female","male", "female","male", "female","male", "female")
))
```

The mean of the random sample is 2.7575694.

The mean of the logical vector is 0.6.

The mean of the character vector is NA.

The mean of the factor vector is NA.

For the random sample and logical vector, means were produced. For the character vector and factor vector, no means were produced.

``` r
question_one_numeric_df = tibble(
  logical_vec_one_numeric = as.numeric(question_one_df$logical_vec_one),
  character_vec_one_numeric = as.numeric(question_one_df$character_vec_one),
  factor_vec_one_numeric =  as.numeric(question_one_df$factor_vec_one)
)
```

    ## Warning in eval_tidy(xs[[i]], unique_output): NAs introduced by coercion

The new mean of the logical vector is 0.6.

The new mean of the character vector is NA.

The new mean of the factor vector is 1.5.
