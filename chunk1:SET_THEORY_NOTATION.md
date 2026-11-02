# Sets

## What is a Set?

- A **well-defined** (there is a definite, unambiguous yes-or-no answer to the question "Is x a member of this set?") collection of **unique** objects (eg: `{1,1,2}` is same as `{1,2}`).
- **Not homogeneous**: eg `{"dog", 3, y}` is a valid set
- The order of elements in a set does not matter
  - `{1,2}` and `{2,1}` are the same set

> **NOTE**: "A set of all short people" cannot be considered a valid set. Because sets have to be well-defined. So calling it a set, with no exact heights at which a person becomes short means we have no perfect accuracy to be able to test the set or if an object is in that set.

# Subsets

## What are Subsets?

- Set A is a subset of set B if every element in A is also in B
- We use the notation `A ⊆ B` to say "A is a subset of B."

### Examples of Subsets

- `{1,2} ⊆ {1,2,3}`
- `{1,2,3} ⊆ {1,2,3}`

### Equivalent Statements

The following two statements are equivalent:

- `A = B`
- `A ⊆ B` and `B ⊆ A`

Two sets are **equal** to each other **if and only if they are subsets of each other.**

# ∈ Notation
∈ means "element of" and ∉ means "not an element of."

So x ∈ A means "x is an element of A"

### Example
S = {{1}, {2}}
Is 1 ∈ S? **NO** Element 1 is not in S but set: {1} is in S

> **NOTE**: Say we have A = {1,2} and B = {{1,2}, {3}}. Then A ∈ B.
>
> **BUT**: It is not true that A ⊆ B, because A's elements are 1 and 2, and neither is an element of B (B's elements are {1,2} and {3}). It *would* be **true** that {{1,2}} ⊆ B, because its only element, {1,2}, is an element of B.

> If we have a statement: If "x ∈ A then x ∈ B" then x does and should not refer to one particular element. So it must hold no matter which element we pick for x

> Example: "if x ∈ {1,2} then x ∈ {1,3} is false. It works for x = 1 but it fails for x = 2, because 2 ∈ {1,2} and 2 ∉ {1,3}.

# Set Builder Notation
Compact way to describe what a set contains
{ x: condition(x) }

### Example
{x: x^2 = 9 } is equivalent to {-3,3}