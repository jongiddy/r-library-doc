### base::complex

Create complex numbers

---
#### `base::complex(length.out: Numeric(1), real: Numeric, imaginary: Numeric): Complex(length.out)`

**Returns**

A vector of `length.out` complex numbers, where each complex number has real part taken from the next value in `real` and imaginary part taken from the next value in `imaginary`. If `real` or `imaginary` are shorter than `length.out`, they are recycled.
---
#### `base::complex(**r**eal: Numeric, **i**maginary: Numeric): Complex`

Equivalent to calling `base::complex(length.out: Numeric(1), real: Numeric, imaginary: Numeric)` with `length.out` equal to the maximum length of the `real` and `imaginary` vectors.
---
#### `base::complex(length.out: Numeric(1), [m]odulus: Numeric, [a]rgument: Numeric): Complex(length.out)`

Return a vector of `length.out` complex numbers, where each complex number has modulus (magnitude) part taken from the next value in `modulus` and argument (phase) part taken from the next value in `argument`. If `modulus` or `argument` are shorter than `length.out`, they are recycled.
---
#### `base::complex([m]odulus: Numeric, [a]rgument = Numeric): Complex`

Equivalent to calling `base::complex(length.out: Numeric(1), modulus: Numeric, argument: Numeric)` with `length.out` equal to the maximum length of the `modulus` and `argument` vectors.
---
#### `base::complex(): Complex(0)`

Return a 0-length vector of type Complex.
---
#### `base::complex(length.out: Numeric(1)): Complex(length.out)`

Return a vector of `length.out` complex zeros
---
