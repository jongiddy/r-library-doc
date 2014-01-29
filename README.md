r-library-doc
=============

R package documentation, rewritten for programmers from other languages

The R documentation for functions typically is a mix of "does this, except if
something, when it does that instead, or if the first argument is missing, do
another version of this". See [`base::diag`](http://stat.ethz.ch/R-manual/R-devel/library/base/html/diag.html) 
for a typical example (and that's one of the better-written examples).

For people used to programming languages where
libraries have a single function signature, or where polymorphism is slightly
readable, this will drive them insane.  Normal R programmers cope by just 
using what worked last time.

Here, we rewrite the function definitions to make the libraries clearer to non-R
programmers

First, a word about types. There are no scalars in R - a single number by itself
is a vector of length 1. Almost everything else is a vector. Multi-dimensional
arrays (including 2-dimensional matrices) are just vectors with an accompanying
description of the dimensions.

Hence, many functions will accept a vector and return a vector, cloning any
additional values such as dimensions and labels. We call these functions
shape-preserving, and indicate them purely by their base types.

The R libraries can be incredibly redundant - we flag up redundancies and suggest
the preferred function.  By the word "prefer", we mean use the preferred
function unless the redundant function is more readable (e.g. for consistency
with documentation or related code).

For each function, we display separate panels containing related function signatures. 
If a parameter name in the signature is in **bold**, it *must* be added as a named parameter. 
If the parameter type is in **bold**, the parameter may be
provided by position or as a named parameter.

For example, one of the signatures for the `base::complex` function is:

base::**complex**(length.out: **Numeric(1)**, **modulus**: Numeric, **argument**: Numeric): Complex(*length.out*)

This signature for the `complex` function means the `length.out` parameter, a numeric vector of length 1, may be specified by adding it as the first positional parameter. Alternatively, any positional parameter can be specified as a named parameter. However, the `modulus` and `argument` parameters, both numeric vectors (of any length), *must* be specified as named parameters.  The return value is a complex number vector of size `length.out`.

Here, we document the most reasonable ways to use the function. However, due to the way these R functions are defined, there are additional ways to call them (e.g. it is possible to provide `modulus` and `argument` as positional parameters to `complex`) but these ways are not a good idea - they obscure the meaning of the function. If you absolutely need to write something weird, or, more likely, read something not documented here, a link to the original description is provided at the end of each function definition.
