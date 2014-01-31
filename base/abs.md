## base::abs

Absolute value

---

base::**abs**(*x*: **Integer**) **->** *result*: Integer[*x*]

base::**abs**(*x*: **Double**) **->** *result*: Double[*x*]


#### Returns
a vector of the indicated type with the same attributes as *x*.

Each element is the absolute value of each element in *x*

*x* | *result*
------|-------
<code>base::is.na(x) &#124; x >= 0</code> | `x`
`x < 0`  | `-x`


---

base::**abs**(*x*: **Complex**)

_This function is redundant: prefer `base::Mod(z: Complex)`_

#### Returns
Double[*x*] - a numeric vector with the same attributes as *x*

Each element is the modulus (magnitude) of each element in `x`

---

base::**abs**(*x*: **Logical**) `->` Integer[*x*]

_This function is redundant: prefer `base::as.integer(x: Logical)`_

#### Returns
Integer[*x*] - an integer vector with the same attributes as *x*

Each element is an integer according to following truth table:

Logical | Integer
-----|--------
`TRUE` |  `1L`
`FALSE` |  `0L`
`NA` | `NA_integer_`

---
