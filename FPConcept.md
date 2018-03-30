## Functional Programming
In computer science, **functional programing** is a **programing paradigm** that treads **computation as the evaluation of mathematical functions** and avoids state and mutatble dat.
It emphasizes the application of the functions, in contracts to the imperative programing style, which emphasizes changes in state.
- Programing paradigm
- Computations = function evaluation
- Avoids state sand mutatble data
- Function composition
- Expression everywhere

## Scala
Scala is a morden multi-paradigm programing language designed to express common programing partterns in a concise, elegant, and type safe way. It smootly integreate features of object-oriented and functional languages.
Scala is also a functional language in the sense that every function is a value.

## Expression vs Statement
A statement changes state, it called for side effect
An Expression produces result

Everything in Scala is an Expression
is this an expression?
```scala
def abs(n: Int): Int
    if (n < 0) -n
    else n
```
Yes!
is this an expression?
```scala
if (n < 0) -n
    else n
```
Yes!

## Function type
Type => Type
examples:
> * Int => String
> * (Int, Int) => Int
> * Int => Int => Int
> * (Int => Int) => Int

## Functional trio
 * map
 * filter
 * reduce(foldleft + foldright)

## Functional literal
loop string as character
```scala
"Jaden" filter { c=> c > 100}
res0: String = en
```

`_` means the very first input of the function
```scala
"Jaden" filter { _ > 100}
res1: String = en
```

`()` is another way to express a function
```scala
"Jaden" filter ( _ > 100)
res2: String = en
```

```scala
"Jaden" map { _.toString.toUpperCase}
res5: scala.collection.immutable.IndexedSeq[String] = Vector(J, A, D, E, N)
```