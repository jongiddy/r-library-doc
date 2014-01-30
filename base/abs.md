### base::abs

Absolute value

---

base::**abs**(*x*: **Integer**) `->` Integer[*x*]

base::**abs**(*x*: **Numeric**) `->` Numeric[*x*]

*Returns* |*x*|

*x* | Output
------|-------
<code>base::is.na(x) &#124; x >= 0</code> | `x`
`x < 0`  | `-x`


---

base::**abs**(*x*: **Complex**) `->` Numeric[*x*]

_This function is redundant: prefer `base::Mod(z: Complex): Numeric`_

*Returns* the modulus (magnitude) of `x`

---

base::**abs**(*x*: **Logical**) `->` Integer[*x*]

_This function is redundant: prefer `base::as.integer(x: Logical): Integer`_

*Returns* an integer according to following truth table:

Logical | Integer
-----|--------
`TRUE` |  `1L`
`FALSE` |  `0L`
`NA` | `NA_integer_`

---
