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

For each function, we display a separate panel for each function signature.  If 
the variable name in the signature is in **bold**, add it as a named parameter. 
If the parameter type is in **bold**, the parameter may be
provided by position or as a named parameter.

For example, one of the signatures for the `base::complex` function is:

---

base::**complex**(length.out: **Numeric(1)**, **modulus**: Numeric, **argument**: Numeric): Complex(length.out)

*Returns* a vector of `length.out` complex numbers, where each complex number has modulus (magnitude) part taken from the next value in `modulus` and argument (phase) part taken from the next value in `argument`. If `modulus` or `argument` are shorter than `length.out`, they are recycled.

---

This signature for this form of the function allows `length.out` to be specified as the first positional parameter. It *must* be a numeric vector of size 1. The arguments `modulus` and `argument` *must* be named parameters, both numeric vectors (of any length).  The return value is a complex number vector of size `length.out`.
