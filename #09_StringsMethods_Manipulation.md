# String Methods and Manipulation

Some methods we will see here are
- toUpperCase()
- toLowerCase()
- startsWith("...")
- endsWith("...")
- trim()
- length: it is an attribute.


Other methods are for example:
- match()
- replace()
- split()

```html

<html>

    <body>
        <h1 id="header">Type Something</h1>
        <input type="text" id="inp"/>
        
        <button onclick="pressed()">Click</button>  //Apparently cannot be in the script
        <p id="output"></p>


        <script type="text/javascript">
            function pressed(){
               var text = document.getElementById("inp").value;
               var text2 = document.getElementById("inp").innerHTML;
              // output.innerHTML = text.toUpperCase()
             //  output.innerHTML = text.toLowerCase()
               //output.innerHTML = text.startsWith("@");
               output.innerHTML = text.endsWith("@");
               output.innerHTML = "You typed " + text.trim().endsWith("@"); //trim spaces before and after.
               console.log(text,text2,output);
               //output.innerHTML = "Bor" //has an impact on what we see in browser
               //output.value = "Bonjour"
               console.log(text.length);
               
                }

        </script>
    </body>

</html>
```


# Problematic

Try to understand better the difference between .innerHTML and .value.
