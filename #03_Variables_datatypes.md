# Variables and Data Types



# Data types

## Primitive datatypes
Java Datatypes.
- string: Anything between " " or ' '. Collection of characters.
- number: 2.0, 1000, -98. 
- boolean: true or false in **lower** case.
- undefined: Variable with no value
- null: null


# Variables
Variables can store values/data.

To declare it you have to use the keyword **var**.

```html
var x = 6;
```

```html
<html>

    <body>
        <h1 id="header">Hello</h1>
        <input type="text" id="inp"/>
        <script type="text/javascript">
          
            var x = 6;// this creates the var x
            x= 9; //this change the value of x
            console.log(x); // will appear in the console only.

        </script>
  
    </body>

</html>
```

## Rules to define a variable
The namae has to:
- be meaningful -> var name ="tim"
- no spaces in variable name -> name_person = "tom"
- any letters and numbers are authorized
- cannot start by a number.

## Playing with variables

```html
<html>

    <body>
        <h1 id="header">Hello</h1>
        <input type="text" id="inp"/>
        <script type="text/javascript">
            //document.write(document.getElementById("header").innerHTML);
            var x = 6;
            x=9
            var name="tim";
            var hello_world= 5;
            hello_world = name;
            console.log(hello_world);
            name = "hello";
            console.log(name);


        </script>


    </body>


</html>

```
Here we are seeiong the dynamic character of JS.
Hello_world is first an int and then like nothing happended it became a string.
This is typipcal behaviour of a **dynamic language**.
