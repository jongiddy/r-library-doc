## base::diag

Create, retrieve or update matrix diagnonals

---
### Create an identity matrix

base::**diag**(*x*: **Numeric(1)**)

base::**diag**(***nrow***: Numeric(1), ***ncol***: Numeric(1))

base::**diag**(***nrow***: Numeric(1))

If `x` is supplied, set `nrow` and `ncol` equal to `x`

If `ncol` is not supplied, set equal to `nrow`

#### Returns
Numeric(*nrow*, *ncol*) - a *nrow* x *ncol* numeric matrix

Each element is 1 if the row and column indices are equal, or 0 otherwise.

---
### Create a diagonal matrix

base::**diag**(*x*: **Numeric.Dim(0...1)**, *nrow*: **Numeric(1)**, *ncol*: **Numeric(1)**)

base::**diag**(*x*: **Numeric.Dim(0...1)**, *nrow*: **Numeric(1)**)

base::**diag**(*x*: **Numeric(2...)**)

If *nrow* is not supplied, set equal to length of *x*

If *ncol* is not supplied, set equal to *nrow*

If *x* is shorter than lesser of *nrow* and *ncol*, it is recycled

#### Returns
Numeric(*nrow*, *ncol*) - a *nrow* x *ncol* numeric matrix

For each element `x[i]`, the matrix element `[i,i]` has the same value. Other values are 0.

---
### Extract a matrix diagonal as a vector

base::**diag**(*x*: **Logical.Dim(2)**)

base::**diag**(*x*: **Integer.Dim(2)**)

base::**diag**(*x*: **Numeric.Dim(2)**)

base::**diag**(*x*: **Complex.Dim(2)**)

base::**diag**(*x*: **Character.Dim(2)**)

base::**diag**(*x*: **Raw.Dim(2)**)

#### Returns
<code>vector(mode = typeof(*x*), length = min(dim(*x*)))</code> - a vector of the same type as the matrix *x* with length equal to the lesser of the matrix dimensions

Each element in position `i` is the matrix element `x[i,i]`. If the matrix row and columns names are identical, the result vector will have the same names, otherwise no names.

---
### Set a matrix diagonal from a vector

base::**diag**(*x*: **Logical.Dim(2)**) **<-** *value*: **Logical.Dim(0)**

base::**diag**(*x*: **Integer.Dim(2)**) **<-** *value*: **Integer.Dim(0)**

base::**diag**(*x*: **Numeric.Dim(2)**) **<-** *value*: **Numeric.Dim(0)**

base::**diag**(*x*: **Complex.Dim(2)**) **<-** *value*: **Complex.Dim(0)**

base::**diag**(*x*: **Character.Dim(2)**) **<-** *value*: **Character.Dim(0)**

base::**diag**(*x*: **Raw.Dim(2)**) **<-** *value*: **Raw.Dim(0)**

`length(value) <= min(dim(x))`

If `length(value) < min(dim(x))` then `value` is recycled (repeated until correct length).

#### Effects

For each element in `value`, elements `x[i,i]` are set to `value[i]`.

---

[R Matrix Diagonals](http://stat.ethz.ch/R-manual/R-devel/library/base/html/diag.html)
