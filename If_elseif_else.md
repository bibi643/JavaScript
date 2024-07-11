# If, Else if, else

It is used to **Check a condition before running a piece of code**.

# Problematic of the course

Here we want to change the color of the header using the input of the user.

```html
if (condition){

}
```
- if condition is true then everything between {} will be executed.
- if true is not check, check else if condition(s).

- else happens anytime if condition is not true or all the above is not verfied. (if plus all the else if)

```html
<html>

    <body>
        <h1 id="header">Hello</h1>
        <input type="text" id="inp"/>
        
        <button onclick="pressed()">Click</button>  //Apparently cannot be in the script
        <script type="text/javascript">
            function pressed(){
                var text = document.getElementById("inp").value;

                if(text ==="red"){
                    document.getElementById("header").style.color = "red";


            }else if(text==="green"){
                document.getElementById("header").style.color = "green";
            } else if(text==="blue"){
                document.getElementById("header").style.color = "blue";
            }



            else {
                document.getElementById("header").style.color = "black";
            }
        }
           

        </script>
    </body>

</html>
```
