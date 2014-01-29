### base::complex

Create complex numbers

---
base::**complex**(length.out: **Numeric(1)**, real: **Numeric**, imaginary: **Numeric**): Complex(*length.out*)

base::**complex**(length.out: **Numeric(1)**, real: **Numeric**): Complex(*length.out*)

base::**complex**(length.out: **Numeric(1)**, imaginary: **Numeric**): Complex(*length.out*)

base::**complex**(length.out: **Numeric(1)**): Complex(*length.out*)

base::**complex**(**real**: Numeric, **imaginary**: Numeric): Complex

base::**complex**(**real**: Numeric): Complex

base::**complex**(**imaginary**: Numeric): Complex

If `length.out` is not provided, set to the longer of any `real` or `imaginary` vector.

If `real` is not provided, set to 0.

If `imaginary` is not provided, set to 0.

*Returns* a vector of `length.out` complex numbers, where each complex number has real part taken from the next value in `real` and imaginary part taken from the next value in `imaginary`. If `real` or `imaginary` are shorter than `length.out`, they are recycled.

---

base::**complex**(length.out: **Numeric(1)**, **modulus**: Numeric, **argument**: Numeric): Complex(*length.out*)

base::**complex**(length.out: **Numeric(1)**, **modulus**: Numeric): Complex(*length.out*)

base::**complex**(length.out: **Numeric(1)**, **argument**: Numeric): Complex(*length.out*)

base::**complex**(**modulus**: Numeric, **argument**: Numeric): Complex

base::**complex**(**modulus**: Numeric): Complex

base::**complex**(**argument**: Numeric): Complex

If `length.out` is not provided, set to the longer of any `real` or `imaginary` vector.

If `modulus` is not provided, set to 1.

If `argument` is not provided, set to 0.

*Returns* a vector of `length.out` complex numbers, where each complex number has modulus (magnitude) part taken from the next value in `modulus` and argument (phase) part taken from the next value in `argument`. If `modulus` or `argument` are shorter than `length.out`, they are recycled.

---

base::**complex**(): Complex(0)

*Returns* a 0-length vector of type Complex.

---


[R Complex Vectors](http://stat.ethz.ch/R-manual/R-devel/library/base/html/complex.html)


