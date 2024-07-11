# Switch Statements.

Basically, we will do the same as if, else if , else but using the switch statement.
It is made of 2 parts:
- switch(variable_to_check)
- case "..."
- break means it stops checking and wont bothered to check other cases.
- default is like else in if statements: if none of the case are verified use default.

- We have simulated an if, else if, else statement using a switch statement.

- Switch is easier to read the else if, but can be applied to one variable, and the cases are one unique value.

- ```html
  <html>

    <body>
        <h1 id="header">Hello</h1>
        <input type="text" id="inp"/>
        
        <button onclick="pressed()">Click</button>  //Apparently cannot be in the script
        <script type="text/javascript">
            function pressed(){
                var text = document.getElementById("inp").value;
                switch(text){
                    case "red":
                        document.getElementById("header").style.color = "red";
                        break;
                    
                    case "blue":
                        document.getElementById("header").style.color = "blue";
                        break;


                    case "green":
                        document.getElementById("header").style.color = "green";
                        break;

                    default:
                    document.getElementById("header").style.color = "black";

                        

                }
            }

  
        </script>

    </body>

</html>
```

# Other example
The user will input their age and wew will return to them if they are an adult or not.

Reminder: Whatever the user types in the input box, it is considered as a string. So it will be needed a conversion.

It will be used **parseInt()**, take the integer value of whatever string we gave.

```html
<html>

    <body>
        <h1 id="header">What is your age?</h1>
        <input type="text" id="inp"/>
        
        <button onclick="pressed()">Click</button>  //Apparently cannot be in the script
        <p id="output"></p>




        <script type="text/javascript">
            function pressed(){
                var text = parseInt(document.getElementById("inp").value);
                var output = document.getElementById("output");



                if (text >18){
                    output.innerHTML = "you are older than 18.";
                }else if (text == 18){
                    output.innerHTML = "you are 18.";
                }
                else{
                    output.innerHTML = "you are not older than 18.";
                }
            }

            
        </script>


    </body>

</html>
```

