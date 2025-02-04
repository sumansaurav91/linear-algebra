# Vector

* **Definition**: Vector is a mathematical object that possesses both magnitude (size) and direction, often represented as an arrow with a defined length signifying its magnitude and the arrowhead indicating its direction

## Key points about vectors

* **Components**: A vector is usually expressed as a list of numbers (components) corresponding to its coordinates in a given space (e.g., a 2D vector might be written as (x, y)). 
* **Magnitude**: The length of the vector, calculated using the Pythagorean theorem in most cases. 
* **Direction**: The arrow's direction, determined by the relative values of its components.

## Linear Combinations, Span and Basic Vectors

* Linear combination of ```v``` and ```w``` can be represnted as ```av + bw``` where ```a``` and ```b``` are scalars.
* The span of ```v``` and ```w``` is the set of all their linear combonations.
* Example ```av + bw```, Let ```a and b``` vary over all real numbers.
* For Vector, think as a arrow. For Point, its a set of vectors

## What does the span of 3D vectors look like?
* Linear combination of ```v```, ```w``` and ```u``` can be represented as ```av + bw + uc``` where ```a```, ```b``` and ```c``` are scslars.
* Linearly dependent: ```u = av + bw```, for some values of ```a``` and ```b```
* Linearly independent: ```w != av``` or ```u != av + bw``` for all values of ```a``` and ```b```

## Technical Definition of Basis
* **Definition**: The basis of a vector space is a set of linearly independent vectors that span the full space.

## Span
* **Definition**: The "span" of a set of vectors is the collection of all vectors that can be created by taking linear combinations of those vectors; essentially, it's the set of all possible vectors you can reach by adding scaled versions of the original vectors together. 

## Interesting Scenario

```
Let's start with the first definition:

Vectors v̄, w̄, ū are linearly independent if av̄ + bw̄ + cū = 0̄ has only the trivial solution a = b = c = 0


* Let's show this implies the second definition:
  - If we rearrange av̄ + bw̄ + cū = 0̄ to ū = (-a/c)v̄ + (-b/c)w̄
  - The only solution being a = b = c = 0 means we can't find any non-zero scalars that make this equation work
  - Therefore ū cannot be written as any linear combination av̄ + bw̄
  - This is exactly what the second definition states

* Now let's show the second definition implies the first:
  - If ū ≠ av̄ + bw̄ for any scalars a and b
  - Then av̄ + bw̄ + cū = 0̄ can only be satisfied when c = 0 (otherwise we could solve for ū)
  - But with c = 0, we get av̄ + bw̄ = 0̄
  - By the same logic applied to v̄ and w̄, this requires a = b = 0
  - Therefore we get a = b = c = 0 as the only solution

So both definitions are equivalent ways of saying the same thing: no vector can be written as a linear combination of the others.
The first definition treats all vectors symmetrically while the second highlights one vector's relationship to the others, but they express the same fundamental concept of linear independence.
```

## More Simpler Explaination

```
* The second definition (ū ≠ av̄ + bw̄) is basically saying "you can't get to ū by mixing v̄ and w̄ together in any way."
* It's like saying "you can't make orange by mixing only blue and green."
* The first definition (av̄ + bw̄ + cū = 0̄ only when a = b = c = 0) is just a more formal, mathematical way of saying the same thing.
* Because if you could make ū from v̄ and w̄, you could rearrange the equation to get zero, which would break the rule.
* Think of it like this: if you could get to ū using v̄ and w̄, it would be like having a recipe that says "2 parts v̄ plus 3 parts w̄ equals ū".
* The first definition is just saying no such recipe exists!
```
## Matrices as Linear Transformation
