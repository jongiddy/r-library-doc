## base::complex

Create complex numbers

---
### Create complex numbers from rectangular co-ordinates

base::**complex**(*length.out*: **Double**, *real*: **Double**, *imaginary*: **Double**)

base::**complex**(*length.out*: **Double**, *real*: **Double**)

base::**complex**(*length.out*: **Double**, ***imaginary***: Double)

base::**complex**(*length.out*: **Double**)

base::**complex**(***real***: Double, ***imaginary***: Double)

base::**complex**(***real***: Double)

base::**complex**(***imaginary***: Double)


If `length.out` is not supplied, set to the length of the longest supplied `real` or `imaginary` vectors.

If `real` is not supplied, set to 0.

If `imaginary` is not supplied, set to 0.

If `real` or `imaginary` are shorter than `length.out[1]`, they are recycled (repeated until the specified length).

#### Returns
Complex(*length.out*[1]) - a complex vector of length `length.out[1]`

Each element is a complex number with real component taken from successive values in `real` and imaginary component taken from successive values in `imaginary`.

---
### Create complex numbers from polar co-ordinates

base::**complex**(*length.out*: **Double**, ***modulus***: Double, ***argument***: Double)

base::**complex**(*length.out*: **Double**, ***modulus***: Double)

base::**complex**(*length.out*: **Double**, ***argument***: Double)

base::**complex**(***modulus***: Double, ***argument***: Double)

base::**complex**(***modulus***: Double)

base::**complex**(***argument***: Double)

If `length.out` is not supplied, set to the length of the longest supplied `modulus` or `argument` vectors.

If `modulus` is not supplied, set to 1.

If `argument` is not supplied, set to 0.

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


