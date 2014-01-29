r-library-doc
=============

R package documentation, rewritten for programmers from other languages

The R documentation for functions typically is a mix of "does this, except if
something, when it does that instead, or if the first argument is missing, do
another version of this".  For people used to programming languages where
libraries have a single function signature, or where polymorphism is slightly
readable, this will drive them insane.  Normal R programmers cope by just 
using what worked last time.

Here, we rewrite the functions to make the libraries clearer.

First, a word about types. There are no scalars in R - a single number by itself
is a vector of length 1. Almost everything else is a vector. Multi-dimensional
arrays (including 2-dimensional matrices) are just vectors with an accompanying
descriptin of the dimensions.

Hence, many functions will accept a vector and return a vector, cloning any
additional values such as dimensions and labels. We call these functions
shape-preserving, and indicate them purely by their base types.

The R libraries can be incredibly redundant - we flag up redundancies and suggest
the preferred function.  By the word "prefer", we mean use the preferred
function unless the redundant function is more readable (e.g. for consistency
with documentation or related code).
