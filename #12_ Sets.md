# Sets

Sets are **unordered collection unique of elements**.
Because of this unique property, we cannot index elements.
We can add elements, delete elements and few other operations.
- .add(value_to_add)
- .delete(value_to_delete): If we delete a value which is not, it returns false.
- .size
- .has(value_to_search)
- .values(): return the values in the order they were inserted in the dataset.

# Basics

## Creation and add element
### Option 1
```html
var _set = new Set() //set is a keyword so to name a set, set, we use _set.
```

```html
<html>

    <body>


       <script>
        var arr = [2,3,4,44,3,2,5,6,6]
        var _set = new Set()
        _set.add(6).add(3).add(6)
        console.log(_set)
       
       </script>

    </body>

</html>
```
This will return a set with 6 and 3. The second 6 is not added because a set is made of unique elements.
### Option 2
Here wew create a set passing the set itself in thesetInstructor.


```html
<html>

    <body>


       <script>
        var arr = [2,3,4,44,3,2,5,6,6]
        var _set = new Set([1,1,1,12,1,1,32])
      
        console.log(_set)
        
        
       
       </script>
            

    </body>



</html>
```

## Presence of an element inside a set.

_SET.HAS(VALUE_TO_LOOK_FOR) >>> BOOLEAN

```html
<html>

    <body>


       <script>
        var arr = [2,3,4,44,3,2,5,6,6]
        var _set = new Set()
        _set.add(6).add(3).add(6)
        console.log(_set.has(3))
       
       </script>

    </body>

</html>
```

# For loop to iterate in a set.
This will returns the values of the set.

```html
<html>

    <body>


       <script>
        var arr = [2,3,4,44,3,2,5,6,6]
        var _set = new Set()
        _set.add(6).add(3).add(6)
        for (var entry of _set.values()){
        console.log(entry)
        }
        
       
       </script>
            

    </body>



</html>

```

# forEach()

```html
<html>
    <body>
       <script>
        
        function test(x){
            if (x =="l"){
                console.log("Found it!")
            }else{
            console.log("Nope")
            }   
        }
        var _set2 = new Set("Hello")

        _set2.forEach(test)
      
        console.log(_set2)
        
       </script>
            
    </body>

</html>
```
_set.forEach(function) means for each element of the set, apply function.
