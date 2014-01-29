### base::abs

Absolute value

---

base::**abs**(*x*: **Integer**): Integer

base::**abs**(*x*: **Numeric**): Numeric

*Returns*

If `x` >= 0, return `x`

If `x` < 0, return `-x`

---

base::**abs**(*x*: **Complex**): Numeric

_This function is redundant: prefer `base::Mod(z: Complex): Numeric`_

*Returns* the modulus (magnitude) of `x`

---

base::**abs**(*x*: **Logical**): Integer

_This function is redundant: prefer `base::as.integer(x: Logical): Integer`_

*Returns*

If `x` is `TRUE`, return `1L`

If `x` is `FALSE`, return `0L`

If `x` is `NA`, return `NA_integer_`

---
