# Logical and Assignment Operators
## Basic operators between 2 elements
Operators allow to make operations on data.
- +
- -
- *
- /
- %: gives the remainder of a division.


## Operators to use on the same variable

- += : x+=5 -> means add 5 to x.
- -=
- *=
- /=
- %=
- ++ : Increment by 1
- --: Decrement by 1

Those operators only work on numbers.

## String concatenation

- String with number

```html
var x =10
var str = "hello"

console.log(str + x) // will return hello10
```
This works because under the hood, 10 is converted into a string.

- String with string

```html
var str2 = "world"
var str = "hello"

console.log(str + str2) // will return helloworld
```

If by mistake we perform an operation which is not allowed like str *3, it will return a NaN value in the console if we print it out.
