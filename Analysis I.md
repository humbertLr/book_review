 # Chapter 1 Introduction
## 1.1 What is Analysis?
objects: numbers, sequences, series, limits, functions, definite integrals, derivatives...
focused more on the **underlying theory** for these objects
questions:
1). What is a real number? Is there a largest real number?
2). How do you take the limit of a squence of real numbers?
3). What is a function?
## 1.2 Why Do Analysis?
One can get into trouble if one applies rules without knowing where they came from and what the limits of their applicablity are.
Example 1.2.1: Diviskon by zero. The cancellation law $ac=bc$ => $a=b$ does not work when $c=0$ .
Example 1.2.2: Divergent series. 
Example 1.2.3: Divergent sequences.
Example 1.2.4: Limiting values of functions.
Example 1.2.5: Interchanging sums.
# Starting at the Beginning: The Natural Numbers
## 2.1 The Peano Axioms
## 2.2 Addition
**Definition 2.1.1** (Informal) A natural number is any element of the set
$${N:=\set{0,1,2,3,4,...}}$$
start with 0 and then counting forward indefinitely

it's an intuitive definition, but leaves many questions unanswered like:
- how do we know we can keep counting dindefinitely, without cycling back to 0
- how do you perform operations such as addition, multipliccation, or exponentiation

define complicated operations in terms of simpler operations
- exponentiation: repeated multiplication
- multiplication: repeated addition
- addition: repeated incrementing (counting forward)

incrementing is a fundamental operation, not reducible to any operation, before learning to add

Two fundamental concepts to define natural numbers:
- zero number
- increment (successor operation) -- n++

**Axiom 2.1**: 0 is a natural number
**Axiom 2.2**: If n is a natural number, then n++ is also a natural number

**Definition 2.1.3**: define 1 to be the number 0++, 2 to be the number (0++)++, 3 to be...
**Proposition 2.1.4**: 3 is a natural number
**Example 2.1.5** wrap-aroud issue, computer overflow its memory and the number will wrap around back to 0

**Axiom 2.3**: 0 is not the successor of any natural number; i.e., we have $n++\neq0$ for every natural number n.
**Proposition 2.1.6** 4 is not equal to 0

**Axiom 2.4**: Different natural numbers must have different successors; i.e., if n, m are natural numbers and $n \neq m$ , then $n++ \neq m++$. Equivalently, if $n++=m++$ then we must 
**Definition 2.2.1 (Addition of natural numbers). 
- 0+m:=m
- (n++)+m:=(n+m)++

**Lemma 2.2.2**: For any natural number n, n+0=n
**Lemma 2.2.3**: For any natural numbers n and m, n+(m++)=(n+m)++

**Proposition 2.2.4** (Addition is commutative). For any natural numbers n and m, n+m=m+n

