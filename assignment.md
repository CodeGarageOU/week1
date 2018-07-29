# Assignment - I


## Question 1

Anand has some distinct integer numbers a<sub>1</sub>, a<sub>2</sub> ... a<sub>n</sub> . Count number of pairs (i,j) such that:

* 1 &le; i &le; n
* 1 &le; j &le; n
* a<sub>i</sub> &lt; a<sub>j</sub>

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

## Question 2

A startup company manufactures calculators. Unfortunately, one of them found to be fake. It has
many bugs. It is adding two numbers without carrying. Example expression 23 + 19 will have result
32 in his calculator. Given an expression in the form a + b, output the result from that calculator

### Input

The first line contains an integer T denote the number of test cases. Each test case contains two integers
a,b in a single line

### Output

For each test case, print answer in a single line

### Example

#### Input

```
2
12 9
25 25
```

#### Output

```
11
40
```

## Question 3

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

## Question 4

There are n villages in a line in an area. There are two kings A and B. A village can be either ruled
by a king (either by A or B) or empty. An empty village is said to be controlled by the king A if it is
surrounded by villages ruled by king A from the left and from the right, same goes for king B. Find out
number of villages that are ruled by King A and King B

### Input

The first line of input contains an integer T denoting the number of test cases.
Following T lines of the input, each line contains a string s denoting the state of the
villages, either ruled by A or B or empty, each character of which can be 'A', 'B' or '.'.

### Output

For each test case, output two space separated integers denoting the number of villages
controlled by King A and B respectively

### Constraints

* 1 &le; T &le; 20
* 1 &le; |s| &le; 10<sup>5</sup>

### Example

#### Input

```
4
A..A..B...B
..A..
A....A
..B..B..B..
```

#### Output

```
4 5
1 0
6 0
0 7
```

## Question 5

Given a matrix in which elements are sorted row wise and column wise find number of negative
numbers in the matrix.

## Question 6

What is the maximum number of squares of size 2x2 that can be fit in a right angled isosceles triangle
of base B

Base is the shortest side of the triangle

### Input

First line contains T, the number of test cases

Each of the following T lines contains 1 integer B

### Output

Output exactly T lines, each line containing the required answer

### Constraints

* 1 &le; T &le; 10<sup>4</sup>
* 1 &le; B &le; 10<sup>4</sup>

### Example

#### Input

```
5
1
2
3
4
5
```

#### Output

```
0
0
0
1
1
```
