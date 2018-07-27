# Assignment - I

## Question 1

There are K nuclear reactor chambers labelled from 0 to K-1. Particles are bombarded onto
chamber 0. The particles keep collecting in the chamber 0. However if at any time, there are
more than N particles in a chamber, a reaction will cause 1 particle to move to the immediate
next chamber(if current chamber is 0, then to chamber number 1), and all the particles in the
current chamber will be be destroyed and same continues till no chamber has number of
particles greater than N. Given K,N and the total number of particles bombarded (A), find the final
distribution of particles in the K chambers. Particles are bombarded one at a time. After one
particle is bombarded, the set of reactions, as described, take place. After all reactions are over,
the next particle is bombarded. If a particle is going out from the last chamber, it has nowhere to
go and is lost.

### Input

The input will consist of one line containing three numbers A,N and K separated by spaces. A will
be between 0 and 1000000000 inclusive. N will be between 0 and 100 inclusive. K will be
between 1 and 100 inclusive. All chambers start off with zero particles initially.

### Output

Consists of K numbers on one line followed by a newline. The first number is the number of
particles in chamber 0, the second number is the number of particles in chamber 1 and so on.

### Example

#### Input

`3 1 3`

#### Output

`1 1 0`

## Question 2

Anand has some distinct integer numbers a<sub>1</sub>, a<sub>2</sub> ... a<sub>n</sub> . Count number of pairs (i,j) such that:

* 1 &le; i &le; n
* 1 &le; j &le; n
* a<sub>i</sub> &le; a<sub>j</sub>

### Input

The first line of the input contains an integerT denoting the number of test cases. The
description of T test cases follows .The first line of each test case contains a single
integer n denoting the number of numbers Alexandra has. The second line contains n space-
separated distinct integers a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>n</sub> denoting these numbers.

### Output

For each test case, output a single line containing number of pairs for corresponding test case.

### Example

#### Input

```
2
2
2 1
3
3 1 2
```

#### Output

```
1
3
```

## Question 3

Given a matrix in which elements are sorted row wise and column wise find number of negative
numbers in the matrix.

