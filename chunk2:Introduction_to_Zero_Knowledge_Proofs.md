# Introduction to Zero Knowledge Proofs (ZKP)

These are algorithms where one party is proving to another party they know the solution to a system of equations without revealing the answer.

**Two parties:**
- **Prover:** party doing the convincing
- **Verifier:** party being convinced

> **NOTE:** ZKP prove KNOWLEDGE, not TRUTH.

# Systems of Equations for Binary Numbers

`x(x − 1) = 0` means "x holds a binary value (0 or 1)".

Adding binary variables can restrict a value's range.

### Example

If x and y are binary and `z = x + y`, then z is an integer from 0 to 2.

### Every Digit Needs Its Own Binary Equation

If we don't enforce, for example, the binary `b0`, then the value of n could be anything.

So if we have:
- `b1(b1 − 1) = 0`
- `b2(b2 − 1) = 0`
- `b3(b3 − 1) = 0`

then in the equation **`8b3 + 4b2 + 2b1 + b0 = n`**, n is not restricted to any value, since `b0` is not enforced.

# Statements about Set Membership
We can use a system of equations to say that a variable has either 0 or 1. We can generalize this to an arbitrary set of values

### Example
Let's create a system of equations with the sematic meaning that :  x ∈ {1,5,16,2}

Answer: `(x - 1)(x - 5)(x-16)(x-2) = 0`


# Statements about Set Equality
If we have: S1 = S2, where S1 and S2 are sets.
So if the sets are equal, then that means every element in S1 is an element in S2 and vice versa.

