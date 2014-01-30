## base::complex

Create complex numbers

---
### Create complex numbers from real and imaginary components

base::**complex**(*length.out*: **Numeric**, *real*: **Numeric**, *imaginary*: **Numeric**)

base::**complex**(*length.out*: **Numeric**, *real*: **Numeric**)

base::**complex**(*length.out*: **Numeric**, ***imaginary***: Numeric)

base::**complex**(*length.out*: **Numeric**)

base::**complex**(***real***: Numeric, ***imaginary***: Numeric)

base::**complex**(***real***: Numeric)

base::**complex**(***imaginary***: Numeric)


If `length.out` is not provided, set to the length of the longest supplied `real` or `imaginary` vectors.

If `real` is not provided, set to 0.

If `imaginary` is not provided, set to 0.

If `real` or `imaginary` are shorter than `length.out[1]`, they are recycled (repeated until the specified length).

#### Returns
Complex(*length.out*[1]) - a complex vector of length `length.out[1]`

Each element is a complex number with real component taken from successive values in `real` and imaginary component taken from successive values in `imaginary`.

---
### Create complex numbers from polar co-ordinates

base::**complex**(*length.out*: **Numeric**, ***modulus***: Numeric, ***argument***: Numeric)

base::**complex**(*length.out*: **Numeric**, ***modulus***: Numeric)

base::**complex**(*length.out*: **Numeric**, ***argument***: Numeric)

base::**complex**(***modulus***: Numeric, ***argument***: Numeric)

base::**complex**(***modulus***: Numeric)

base::**complex**(***argument***: Numeric)

If `length.out` is not provided, set to the length of the longest supplied `modulus` or `argument` vectors.

If `modulus` is not provided, set to 1.

If `argument` is not provided, set to 0.

The `argument` parameter is an angle, measured in radians.

If `modulus` or `argument` are shorter than `length.out[1]`, they are recycled (repeated until the specified length).

#### Returns
Complex(*length.out*[1]) - a complex vector of length `length.out[1]`

Each element is a complex number with modulus (magnitude) taken from successive values in `modulus` and argument (phase), in radians, taken from successive values in `argument`.

---

base::**complex**()

#### Returns
Complex(0) - a complex vector of length 0

This vector has no elements, but has "complex" mode.

---


[R Complex Vectors](http://stat.ethz.ch/R-manual/R-devel/library/base/html/complex.html)


