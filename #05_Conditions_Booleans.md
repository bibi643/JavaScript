# Conditions and Booleans

- Booleans defintion
var b = true
var c = false

**Note**: True and False are not allowed with capital T and F.

Booleans are used in general for comparison purpose. In that case we use comparison operators.

# Comparison Operators
- >
- <
- >=
- <=
- == : equivalent operator
- != : Not equal to, opposite of **==**
- !==: opposite of **===**
- ! : not

Note: 
- = is the *assignment* value
- === equivalent in value **and** in types.


```html
<html>

    <body>
        <h1 id="header">Hello</h1>
        <input type="text" id="inp"/>
        <script type="text/javascript">
          
            var x = 7
            var y = 10
            var b = x < y;
            console.log(b);
            
        </script>
    </body>
</html>

```

- AND &&: If **both are true**, it will return true.
- OR ||

Note: If we have a bunch of || || && && && || &&, AND conditions are evaluated first, as multiplcations are first evaluted over additions for example.

```html
<html>

    <body>
        <h1 id="header">Hello</h1>
        <input type="text" id="inp"/>
        <script type="text/javascript">
        
            var name = "tim";
            var other_name= "Tim";
            var x = 10;
            var y = 11;
   
            console.log(name == other_name && y < x);

        </script>
    </body>

</html>
```
