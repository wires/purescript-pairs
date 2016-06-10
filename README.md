purescript-pairs
================

This module defines a datatype `Pair` and a few useful instances and helper
functions. Note that this is not just `Tuple a a` but rather a list with
exactly two elements. Specifically, the `Functor` instance maps over both
values in contrast to the `Functor` instance for `Tuple`.

Example
-------

``` purescript
> let point1 = 2 ^ 3
> let point2 = 4 ^ 7

> sum point
5

> (+) <$> point1 <*> point2
(6) ^ (10)
```