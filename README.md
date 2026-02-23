# MAMBO

MAMBO is achronym for Matrix A, Matrix B operations. A calculator to solve Basic Operations over Matrices like $A \times B$, $A + B$ etc. This is aExecutable  CLI Terminal Binary Made with Rust.

## Features

Import x Export matrices from file
CLI operations 
Algebric operations
Algebric reduction and simplification for incognitoes

## Usage

```cmd
mambo -A 1 0 0 1 -B 0 1 1 0 --solve A + B > A.matrix
```

read A and B from file
```cmd
mambo -F A.matrix A.matrix --solve A + B
```

## Support Operations

A + B
A * B
A * 22/7

## Algebric simplification

Matrices can have unknown variables. Avoid spaces between expressions
```cmd
mambo -A 2x+b 3x+b 0 1 -B 0 1 1 0 --solve A + B | x=i b=9 > A.matrix
```

## Matrix Generation Function

```cmd
mambo -A formula 2*i+j
```

## Conditionals

```cmd
mambo -A formula if i==j then 2*i+j else 0 -B 1
```

## Shape

To generate from formula could be necessary to fill shape of matrices

```cmd
mambo --shape 2x3 3x2
```

Similar meaning
shape 2,3
shape(2, 3)
