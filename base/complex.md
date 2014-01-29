### base::complex

Create complex numbers

---
base::**complex**(length.out: **Numeric(1)**, real: **Numeric**, imaginary: **Numeric**): Complex(*length.out*)

*Returns* a vector of `length.out` complex numbers, where each complex number has real part taken from the next value in `real` and imaginary part taken from the next value in `imaginary`. If `real` or `imaginary` are shorter than `length.out`, they are recycled.

---
base::**complex**(length.out: **Numeric(1)**, real: **Numeric**): Complex(*length.out*)

*Returns* a vector of `length.out` complex numbers, where each complex number has real part taken from the next value in `real` and zero imaginary part. If `real` is shorter than `length.out`, it is recycled.

---

base::**complex**(**real**: Numeric, **imaginary**: Numeric): Complex

Equivalent to calling `base::complex(length.out: Numeric(1), real: Numeric, imaginary: Numeric)` with `length.out` equal to the maximum length of the `real` and `imaginary` vectors.

---

base::**complex**(length.out: **Numeric(1)**, **modulus**: Numeric, **argument**: Numeric): Complex(*length.out*)

*Returns* a vector of `length.out` complex numbers, where each complex number has modulus (magnitude) part taken from the next value in `modulus` and argument (phase) part taken from the next value in `argument`. If `modulus` or `argument` are shorter than `length.out`, they are recycled.

---

base::**complex**(**modulus**: Numeric, **argument**: Numeric): Complex

Equivalent to calling `base::complex(length.out: Numeric(1), modulus: Numeric, argument: Numeric)` with `length.out` equal to the maximum length of the `modulus` and `argument` vectors.

---

base::**complex**(): Complex(0)

*Returns* a 0-length vector of type Complex.

---

base::**complex**(length.out: **Numeric(1)**): Complex(*length.out*)

*Returns* a vector of `length.out` complex zeros

---
