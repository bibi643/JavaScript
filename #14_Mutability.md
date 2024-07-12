# Mutability

Changeable or not changeable concept.

- **Primitive datatype**:
  - are immutable
  - are referencing values rather than object.
  - ex: var x = 5
 ```html
<html>

    <body>


       <script>
        
       var x =5
       var t = x //if change t it does not affect x.

       function add5(num){
        num +=5
        console.log(num)
       }
       
        add5(x)//retunr 10 obvio
        console.log(x) // x did not changed
       
       </script>
            

    </body>

</html>
```
x did not change because var is a primitive datatype so we are putting in the fucntion a kind of a coppy of the variable x. Not the actual x.



Whereas object are mutable such as arrays [] or sets {}.
Here because wew are passing an array as parameter, and arrays are mutable object, we are in fact passing the real object into the function. So it will be affected.

```html
<html>

    <body>


       <script>
        
     

       function append5(arr){
        arr.push(5)
        console.log(arr)
       }
       
        
       var x = [1,2,3,4]
        append5(x)
        console.log(x) 
       
       </script>
            

    </body>



</html>
```


Basically when we do
```html
arr_1 = []
arr_2 = arr_1
```
arr_1 creates a pointer to the location of arr_1.
arr_2 is not copying the values of the array, we are copying the pointer to the location of arr_1.

So **how to actually copy an array**?
**Copy** means we can later modify the copy and this will not affect the original.

```html
<html>

    <body>

       <script>
        
       
    //Method 1
       var x = [1,2,3,4]
       var y = x.slice()
       var z = x.slice(0,2)
       y[2]=999
       console.log(x) 
       console.log(y)


    // Method 2

    var c = [...x]
    y[2]=999
    console.log(x) 
    console.log(y)

       
       </script>
            

    </body>

</html>
```



