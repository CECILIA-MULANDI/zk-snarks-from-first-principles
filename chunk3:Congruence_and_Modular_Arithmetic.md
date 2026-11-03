# A First Definition of Congruence

Given two numbers a and b, we say that a is congruent to b mod q if they both have the same remainder after being divided by q.

`a ≡ b (mod q)`

### Example

Given 5 and 9 mod 4. We say that they are congruent to each other mod 4 because:
- 5 / 4 = 1 rem **1**
- 9 / 4 = 2 rem **1**
- 1 is the remainder for both, i.e. `5 ≡ 9 (mod 4)`

# Set of Unique Numbers in Congruence

In modular arithmetic mod q, only the set of numbers `{0, 1, 2, 3, ..., q − 1}` exists.

### Example

Given mod 5, we only have the following set of numbers:
- `{0, 1, 2, 3, 4}`

So if we got a number like 9, we have to first find `9 (mod 5) = 3`. Meaning we'd be looking for 3, not 8.

# Addition in Modular Arithmetic

We do addition like we would normally, then take that sum and compute the congruence.

`x + y (mod q)`

### Example

Given `3 + 4 (mod 5)`:
- 3 + 4 = 7, and 7 mod 5 = 2
- Hence: `3 + 4 ≡ 2 (mod 5)`

# Modular Multiplication

We do multiplication like we would normally, then take that product and compute the congruence.

`x · y (mod q)`

### Example

Given `3 · 4 (mod 5)`:
- 3 · 4 = 12, and 12 mod 5 = 2
- Hence: `3 · 4 ≡ 2 (mod 5)`