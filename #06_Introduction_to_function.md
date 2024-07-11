# Introduction to function

This chapter is a brief introduction to function.

Definition:

Piece of code that do something.
A function should do one thing and very well and we can reuse the code multiple times.

# Creation

```html
function function_name(){
things to do
...
...
}
```

# Parameters and return statements.

Parameters are informations I need to pass to my function.

```html
function function_name(){
things to do
...
...
}
```
```html
<html>

    <body>
        <h1 id="header">Hello</h1>
        <input type="text" id="inp"/>
        <button>Green</button>
        <button>Red</button>  //Apparently cannot be in the script
        <script type="text/javascript">
            function add(a,b){
                return a + b;
            }
            var x = add(5,5); //call the function and store the result in a variable
        
            var y = add(8,7);

            console.log(x,y);
            console.log(add(87,65));

        </script>

    </body>

</html>

```

**What happens if the function has no return statement?**
```html
<html>

    <body>
        <h1 id="header">Hello</h1>
        <input type="text" id="inp"/>
        <button>Green</button>
        <button>Red</button>  //Apparently cannot be in the script
        <script type="text/javascript">

            function add(a,b){
                console.log(a+b) ;
            }
            add(5,5);

        </script>

    </body>

</html>
```
This will still work because we are printing in the console from inside the function.



# Calling a function from the HTML website.
```html
<html>

    <body>
        <h1 id="header">Hello</h1>
        <input type="text" id="inp"/>
        <button onclick="green()">Green</button>
        <button onclick="red()">Red</button>  //Apparently cannot be in the script
        <script type="text/javascript">

            function red(){
                console.log("red") ;
            }

            function green(){
                console.log("green") ;
            }
           
        </script>

    </body>

</html>
```
```html
<button onclick="red()">Red</button>
```
This means that we create a button called **Red** and when we click on it (onclick) it will run the function red().

- Now we will change the header, depending where we click. We will also change the color.

```html
<html>

    <body>
        <h1 id="header">Hello</h1>
        <input type="text" id="inp"/>
        <button onclick="green()">Green</button>
        <button onclick="red()">Red</button>  //Apparently cannot be in the script
        <script type="text/javascript">

            function red(){
                console.log("red") ;
                document.getElementById("header").innerHTML="RED";
                document.getElementById("header").style.color="red";
            }

            function green(){
                console.log("green");
                document.getElementById("header").innerHTML="GREEN";
                document.getElementById("header").style.color="green"  ;
            }

        </script>
    </body>
</html>
```

Basically when we click on a button the function we call is:
- grabbing the header element (getElementById)
- get what is inside (innerHTML) and name it Green or Red.
- change the color of this element which is in the Header (style.color)
