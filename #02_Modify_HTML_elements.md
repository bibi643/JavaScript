# Modifying HTML Elements

Here we want to modify the <h1>, so we can add an id.
<h1 id="header">Hello</h1>
If I want to reference  the h1 I will use the document and not the console.

*document.getElementById("header").innerHTML = whatever_you_want*

innerHTML means get what is between the tags.

To get the element just and write it just type without any assignation as before

*document.write(document.getElementById("header").innerHTML)* 

```html
<html>
    <body>
        <h1 id="header>Hello</h1>
        <script type="text/javascript">
          document.getElementById("header").innerHTML = "Tech With Tim";
          document.write(document.getElementById("header").innerHTML);
          console.log( document.getElementById("inp").value) //To send in the console the value of the id "inp"
        
        </script>
     

    </body>

</html>

```

# Comments
In JS comments are made like in Go.

