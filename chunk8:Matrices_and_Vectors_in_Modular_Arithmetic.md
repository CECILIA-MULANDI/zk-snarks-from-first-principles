# Vector and Matrix Addition in Modular Arithmetic

Vectors are added element-wise, then each element is reduced mod q:

```
⎡ a₁ ⎤   ⎡ b₁ ⎤   ⎡ (a₁ + b₁) mod q ⎤
⎢    ⎥ + ⎢    ⎥ ≡ ⎢                 ⎥   (mod q)
⎣ a₂ ⎦   ⎣ b₂ ⎦   ⎣ (a₂ + b₂) mod q ⎦
```


# Hadamard Product

Given two vectors, the Hadamard product (⊙) is their element-wise product.

Only valid if both vectors have the same dimensions.

For two vectors `a` and `b`:

```
⎡ a₁ ⎤   ⎡ b₁ ⎤   ⎡ a₁ ⋅ b₁ ⎤
⎢ a₂ ⎥ ⊙ ⎢ b₂ ⎥ = ⎢ a₂ ⋅ b₂ ⎥
⎣ a₃ ⎦   ⎣ b₃ ⎦   ⎣ a₃ ⋅ b₃ ⎦
```


# Inner Product in Modular Arithmetic/ dot product

The inner product of two vectors `a` and `b` of length `n` is:

```
          n−1
⟨a, b⟩ =   ∑   aᵢ ⋅ bᵢ   (mod q)
          i=0
```

### Example

Compute the inner product of the following vectors modulo 7, without a calculator:

```
⟨ ⎡ 2 ⎤ , ⎡ 4 ⎤ ⟩   (mod 7)
  ⎣ 3 ⎦   ⎣ 5 ⎦
```

First, the element-wise products:
- `2 ⋅ 4 = 8`
- `3 ⋅ 5 = 15`

Then sum them: `8 + 15 = 23`

Finally, take the modulus: `23 ≡ 2 (mod 7)`

Therefore, the inner product is **2**.

# Matrix Multiplication with a Vector

Multiplying a matrix by a vector can be interpreted as the inner product of the matrix's columns with the vector.

### Example

```
⎡ 1  2 ⎤ ⎡ 7 ⎤   ⎡ 1 ⎤       ⎡ 2 ⎤
⎢      ⎥ ⎢   ⎥ = ⎢   ⎥ ⋅ 7 + ⎢   ⎥ ⋅ 8
⎣ 3  4 ⎦ ⎣ 8 ⎦   ⎣ 3 ⎦       ⎣ 4 ⎦
```

Written as an inner product of the column vectors with the coefficients:

```
      ⎡ ⎡ 1 ⎤   ⎡ 2 ⎤ ⎤
  = ⟨ ⎢ ⎢   ⎥ , ⎢   ⎥ ⎥ , [ 7, 8 ] ⟩
      ⎣ ⎣ 3 ⎦   ⎣ 4 ⎦ ⎦
```

You might also understand this as a "linear combination of the columns using the coefficients of the vector." Both mean exactly the same thing.