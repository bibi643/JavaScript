# Arrays
Arrays are **ordered collection of elements**.


# Creation of arrays
```html
var tim = 5;
```
This variable stores only one elements.

To store multiiple elements, we use [].

```html
tim2 = [3,4,5,"tom","Hello"]

```
Note how this array can have multiple data type in it.

# Accessing element using indexes.

Indexes are integers that represent the position of the element in  the array.

```html
console.log(tim2[2])
```
# Changing elements of an array

```html
tim2[1]= "new element"
```

# Length property of an array (.length())
```html
tim2.length
```
# Remove/Push the last element (.pop(), push())

- pop()

```html
tim2.pop()
console.log(tim2) 
```
**Be careful**: This will return the array without the last element.

**VS**

```html
console.log(tim2.pop())
console.log(tim2)
```

This will return the eliminated element and on the next  line the array without the eliminated element.

- push()

```html
tim2.push(300)
```
This will add 300 at the end of the array

# Remove first element (shift())
Behave the same way as pop()
First line will return the element we removed.
Second line will return the new array.
```html
  console.log(tim2.shift())

  console.log(tim2)
```

# sort an array

```html
tim2.sort()
```


# Bonus
For now the array is made of 5 elements.

If we add an element to the index 10 for example, the array will be filled by 0 where it is necessary.

```html
tim2[12]= 21
console.log(tim2)
```


# Script

```html
<html>

    <body>


       <script>
        var tim = 5;
        var tim2 = ["hello", 5, 6, 7, "tom"]
        console.log(tim2[2])
        tim2[0]= 23
        console.log(tim2)
        console.log(tim2.pop())

        console.log(tim2)

        console.log(tim2.push(300))

        console.log(tim2)

        console.log(tim2.shift())

        console.log(tim2)

       
        tim2[12]= 21
        console.log(tim2)

       </script>
            
    </body>

</html>

```
