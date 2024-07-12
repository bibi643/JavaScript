# Loops
Here we will see both types of loops

- While: Loop that will run **while a condition is true**.

```html
while(condition){}
```
To avoid infinite loop we need to write an exit.
- For


# While loop

- Example 1:

```html
<html>

    <body>


       <script>
        var i = 0
        while(i <10){
            console.log(i)
            i ++


        }
      
       </script>
            
    </body>

</html>
```

- Example 2: When we need a condition to be true, we may want to exit the loop at a certain point -> **break**.
  

```html
<html>

    <body>


       <script>
        var i = 0
        while(true){
            console.log(i)
            i ++
            if (i == 5){
                break
            }


        }
        console.log("BREAK")
      
       </script>
            
    </body>


</html>
```

In this example it will print i and then after break the loop it will print BREAK. The print of BREAK is outside the loop.
**IMPORTANT TO REMEMBER**:
When you use a while loop you either have:
  -   a condition that will be false at some point so you exit the loop.
  -   break keyword to break the loop at some point.


- Example 3: While loop with arrays.
**Looping inside the array**
```html
<html>

    <body>


       <script>
        var arr = ["tim","joe","bill"]
        var i =0
        while(i < arr.length){
            console.log(arr[i])
            i ++
            


        }
       

       </script>

    </body>

</html>
```


**Creating an array using while loop**.

```html
<html>

    <body>


       <script>
        var arr = ["tim","joe","bill"]
        var i =0
        while(i <= 100){
            arr.push(i)
           
            i ++
    
        }
        console.log(arr)
       
       </script>

    </body>

</html>

```

# Do while loop

```html
var cond =false
while (cond){
...}
```
This will never run because the condition is false since the beginning.


```html
var cond = false
do {
console.log("run")
} while (cond)
```
This means, **whatever the condition is, do {this} at least one time and THEN check the condition.**


```html
<html>

    <body>


       <script>
        var arr = ["tim","joe","bill"]
        var cond =false
        do{
            console.log("RUN")

        }while(cond)
         
       </script>

    </body>
</html>
```


# For loop
**Most common loops** in programming. You use it when you want to loop a specific amount of time.

*General syntax*

```html
for(variable; condition; increment_step){}
```


```html
<html>

    <body>
       <script>
        for (var i = 0; i<10; i++){
            console.log(i)
            if (i==7){
                break //this break the for loop when we reach 7
            }
        }

       </script>

    </body>

</html>
```

## Loop in an array.
We will create a function to look inside an array for a value and return true or false if the value is the one we want.

```html
<html>

    <body>


       <script>
        function findArray(arr,value){
            for (var i=0;i<arr.length;i++){
                if(arr[i] == value){
                    return true
                }
            }

            return false



        }
        var arr = [1,2,4,5,"tim",true]
        console.log(findArray(arr,5))
    
       </script>

    </body>

</html>
```

## Nested for loop

We will write a function to print how many times a function ran.
```html
<html>

    <body>


       <script>
        function findArray(arr,value){
            for (var i=0;i<arr.length;i++){
                if(arr[i] == value){
                    return true
                }
            }

            return false



        }
        var arr = [1,2,4,5,"tim",true]
        console.log(findArray(arr,5))
    
        function nsquared(n){
            for(var i=0;i<n;i++){
                for (var j =0; j<n;j++){
                    console.log("run")
                }
            }
            
        }

        nsquared(5)
       </script>
            
    </body>

</html>
```

## For Of/For Each loops
This is a way to iterate by **elements or items** rather than by *index*. This is the same phylosophie as python does the for loop.
for(let **element** of array) means each element of the array on each loop will be assignated to the **element variable**.

```html
<html>

    <body>


       <script>
        var arr = ["tim","joe","bill"]
        console.log(arr)
        for (let element of arr){
            console.log(element)
            element=5
            console.log(element)
        }
        console.log(arr)
       </script>
            
    </body>

</html>
```

- Loop on a string.

```html
<html>

    <body>


       <script>
        var x ="hello"
        for(let letter of x){
            console.log(letter)
            
        }
       </script>
            
    </body>

</html>
```
**Note**: In the console we will have:
- h
- e
- l      **(2)**
- o

