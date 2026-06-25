# Line & Vector Analysis

A Python project for analytical geometry and vector analysis

## Overview

This project implements fundamental concepts of analytical geometry and linear algebra, including:

* Line equation generation from two points
* Line intersection detection and classification
* Vector dot product calculation
* Cosine similarity analysis
* Geometric interpretation of vector relationships
* 2D and 3D visualization using Matplotlib

The program can determine whether two lines are:

* Intersecting
* Parallel
* Identical

It can also analyze vectors and determine whether they are:

* In the same direction
* Opposite directions
* Orthogonal (90°)
* Forming an acute angle
* Forming an obtuse angle

---

## Features

### Line Analysis

* Generate a line equation from two points.
* Represent lines in the standard form:

[
ax + by + c = 0
]

* Detect geometric relationships between two lines.
* Compute the exact intersection point using determinants (Cramer's Rule).
* Visualize lines and intersection points.

### Vector Analysis

* Compute the Dot Product.
* Compute Cosine Similarity.
* Interpret vector relationships geometrically.
* Support both 2D and 3D vectors.
* Visualize vectors graphically.

---

## Technologies Used

* Python
* NumPy
* Matplotlib




---

## Mathematical Concepts

### Line Equation

Given two points:

```python
P1(x1, y1)
P2(x2, y2)
```

The line coefficients are calculated as:

```python
a = y1 - y2
b = x2 - x1
c = x1*y2 - x2*y1
```

Resulting in:

```text
ax + by + c = 0
```

### Dot Product

```python
dot = np.dot(v1, v2)
```

### Cosine Similarity

```python
cosine = dot / (||v1|| × ||v2||)
```

Interpretation:

| Cosine Value | Meaning            |
| ------------ | ------------------ |
| 1            | Same Direction     |
| 0            | Orthogonal         |
| -1           | Opposite Direction |
| > 0          | Acute Angle        |
| < 0          | Obtuse Angle       |

---

## Example Output

### Line Analysis

```text
Line 1: -4x + 3y - 2 = 0
Line 2: 4x + 3y - 22 = 0

Relation: Intersecting
Intersection Point: (2.50, 4.00)
```

### Vector Analysis

```text
Vector 1: [3,4]
Vector 2: [-4,3]

Dot Product: 0
Cosine Similarity: 0.0000
Interpretation: Orthogonal (90°)
```

---

## Educational Objectives

This project demonstrates:

* Analytical Geometry
* Linear Algebra
* Determinants
* Vector Operations
* Numerical Computing with NumPy
* Scientific Visualization with Matplotlib


