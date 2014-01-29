### base::abs

Absolute value

---

base::**abs**(*x*: **Integer**): Integer

base::**abs**(*x*: **Numeric**): Numeric

*Returns* `-x` when `x < 0`, else `x`

---

base::**abs**(*x*: **Complex**): Numeric

_This function is redundant: prefer `base::Mod(z: Complex): Numeric`_

*Returns* the modulus (magnitude) of `x`

---

base::**abs**(*x*: **Logical**): Integer

_This function is redundant: prefer `base::as.integer(x: Logical): Integer`_


When | Returns
-----|--------
`x == TRUE` |  `1L`
`x == FALSE` |  `0L`
`base::is.na(x)` | `base::NA_integer_`

---
