## base::diag

Create, retrieve or update matrix diagnonals

---
### Extract a matrix diagonal as a vector

base::**diag**(*x*: **A.Dim(2)**)

#### Returns
A.Dim(0) - a vector of the same type as the matrix *x* with length equal to the lesser of the matrix dimensions

Each element in position `i` is the matrix element `x[i,i]`. If the matrix row and columns names are identical, the result vector will have the same names, otherwise no names.

---
### Set a matrix diagonal from a vector

base::**diag**(*x*: **Atomic.Dim(2)**) <- value: Atomic.Dim(0)

`length(value) <= min(dim(x))`

If `length(value) < min(dim(x))` then `value` is recycled (repeated until correct length).

#### Effects

For each element in `value`, elements `x[i,i]` are set to `value[i]`.

---
### Create an identity matrix

base::**diag**(***nrow***: Numeric(1), ***ncol***: Numeric(1))

base::**diag**(***nrow***: Numeric(1))

base::**diag**(*x*: Numeric(1))

If `x` is supplied as a vector or 1-dimensional array, set `nrow` and `ncol` equal to `x`

If `ncol` is not supplied, set equal to `nrow`

#### Returns
Numeric(*nrow*, *ncol*).Dim(2) - a *nrow* x *ncol* numeric matrix

Each element is 1 if the row and column indices are equal, or 0 otherwise.
