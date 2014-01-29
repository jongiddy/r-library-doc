## `base::abs`


### `base::abs(x: Integer): Integer`

### `base::abs(x: Numeric): Numeric`

If `x` >= 0, return `x`

If `x` < 0, return `-x`

### `base::abs(x: Complex): Complex`

Return the modulus of `x`

_Note, this function is redundant: prefer `base::Mod(z: Complex)`_

### `base::abs(x: Logical): Integer`

If `x` is `TRUE`, return `1L`

If `x` is `FALSE`, return `0L`

If `x` is `NA`, return `NA_integer_`

_Note, this function is redundant: prefer `base::as.integer(x: Logical)`_
