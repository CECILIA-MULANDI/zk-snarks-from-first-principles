# Multiplicative Inverses in Modular Arithmetic

Given x, the multiplicative inverse of x is a  number y s.t x * y ≡ 1

# Multiplying Additive Inverses

Numbers close to the modulus `q` are congruent to small negative numbers:

- `q − 1 ≡ −1`
- `q − 2 ≡ −2`
- `q − k ≡ −k` in general

So if **both** numbers are close to `q`, convert each to its negative equivalent first, then multiply. The two negatives cancel and you only multiply small numbers.

### Example

Given q = 101, compute `99 ⋅ 98 (mod 101)`:
- `99 ≡ −2` and `98 ≡ −3`
- `(−2) ⋅ (−3) = 6`
- So `99 ⋅ 98 ≡ 6 (mod 101)`