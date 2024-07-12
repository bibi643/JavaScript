# Maps
Maps are kind of mixture between sets and arrays.
To create a new map, just run this.
var mp = new Map()

It takes keys:values pairs like dictionnaries.

# maps Operation
To initiate a map with values in it. we need to pass insdie the Map instructor an array of arrays(key,values pairs).

- add a value.
  To add a new value, map_name.set("New_key", "new_value")

- To replace a value

To replace a value, map_name.set("**Existing**_key", "new_value")

- get a value
To get a value, we access through the key using map_name.get("key_value")

- Size of the map.

  **map_name.size** will return the number of keys of the map.

- delete keys

map_name.delete("key_to_delete")

- **has** will return a boolean if the **value** we want is inside the map.

map_name.has(6)


- entry. is the key value pair. I think it is like items in python dictionnaries.

To access the key just type entry_name[0]
To access the value just type entry_name[1]

## Script

```html
<html>

    <body>


       <script>
        
        var mp = new Map(
            [
            ["t",5],
            ["v",8]
        ])
        mp.set("t", 9)
        mp.set("w",10)
        console.log(mp.get("v"))
        console.log(mp.has("10"))
        for (var entry_name of mp){
            console.log(entry_name)
            console.log(entry_name[0])
            console.log(entry_name[1])
        }

       </script>

    </body>
</html>
```

# example of why to use a map.

How many t's, how many l's in a string.

```html
<html>

    <body>


       <script>
        
        var mp = new Map()
        str = "This is my new string Hello"
        for (var letter of str){
            if(mp.has(letter)){
                mp.set(letter,mp.get(letter)+1)

            }else{
                mp.set(letter,1)
            }
        }
           
        console.log(mp)
        console.log(mp.get("t"))
        
       </script>

    </body>

</html>


```







