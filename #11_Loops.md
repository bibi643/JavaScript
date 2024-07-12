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


