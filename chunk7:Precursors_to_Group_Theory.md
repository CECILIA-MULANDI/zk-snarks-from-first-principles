# Binary Operators

A mathematical operation that takes 2 elements of a set and returns a single element as a result.

> **NOTE**: Unary operators like negation take a single input, eg 5 gives us -5, hence **NOT A BINARY OPERATOR**.

# Closure

Binary operator is closed iff it takes two elements in a set and always returns another element from the set.

### Example

In a set of integers, addition is a closed binary operator because adding any two integers always returns another integer.

# Associativity

A binary operator (⋆) is associative if for all elements a, b, c:

`a⋆(b⋆c) = (a⋆b)⋆c`

# Magma

A set with closed binary operator.

So we need:
1. A set
2. A closure (so any binary operator on two elements must return an element in the set)

# Semigroup

A set that has a binary operator that is both closed and associative.

Every semigroup is a magma but not every magma is a semigroup.

### Example

The set of integers with addition is a semigroup because:

- Addition is closed on integers (adding two integers always gives an integer)
- Addition is associative: `a+(b+c) = (a+b)+c`

# Identity Element

Given S as a set and ⋆ as its binary operator, an element e is the identity iff for all elements `a∈S`:

`a⋆e = a` and `e⋆a = a`

### Example

For addition, 0 is the identity element for any a because:
- `a+0 = a` and `0+a = a`

For multiplication, the identity element is 1 for any element a because:
- `a⋅1 = a` and `1⋅a = a`

# Monoids

A semigroup with an identity element.

It satisfies three properties:
1. **Closure:** The operator always returns an element in the set
2. **Associativity:** `a⋆(b⋆c) = (a⋆b)⋆c`
3. **Identity:** There exists an element e such that `a⋆e = a` and `e⋆a = a` for all a

Every monoid is a semigroup but not every semigroup is a monoid.

# Proof that Identity Elements are Unique


The identity element in a monoid is unique.

Let u be an element in the set s.t for every element a, `u < a`.

#### Example

let u = 3 and we have `{3,16,21}`, hence `u < a` where 3 < 16, 3 < 21.

Then can we have another element w s.t `w < a` for any a in the set. Hence we introduce some new element w that less than every other element in the set `{3, w, 16, 21}`.

Hence "less than every other element" phrasing forces u to be unique.

We can derive a contradiction: Suppose u and w are both minimum elements.

- If that is the case, then u is less than every element, so `u < w`
- It also holds that `w < u`, since w is less than every element

However, `u < w` and `w < u` is a mathematical contradiction, so the premise must be false, and it cannot be the case that both u and w are minimum elements.