# Elliptic Curve Definition

An EC is a set of (x, y) points that satisfy `y² = x³ + ax + b`.

In practice, a is often set to 0 and b to a non-zero number, giving the common form `y² = x³ + b`.

# Horizontal Symmetry of Elliptic Curves

ECs are horizontally symmetric about the x-axis.

If (x, y) is a point, then so is (x, −y).

# Vertical Lines and Elliptic Curves

A vertical line `x = c` can meet the curve in:
- **0 points:** the line misses the curve entirely
- **1 point:** the line touches where y = 0, i.e. (c, 0)
- **2 points:** (c, y) and (c, −y), mirror images by symmetry

A vertical line never hits more than 2 points.