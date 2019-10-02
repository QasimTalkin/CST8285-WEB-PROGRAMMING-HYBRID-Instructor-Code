### Static vs Dynamic Pages. 
* contents dont change unless source code has been edited for static pages as for dynamic pages the the content changes without having to alter the source code. 

### Client side web programing and Server side web programing. 

* Client side runs code on the client side (browser) and server side on the server. 
* They run private from one another. 

| Client     | Server |
| ----------- | ----------- |
| Browser      | server      |
| languages : Js, Jq...   | Languages: PHP (Larvel, cakephp), Ruby on rails, python, c# |
| Direct browser access | no direct browser access |
|unreliable(script can be manipulated) |Reliable(user has no access)|

### JavaScript

**NOT RELATED TO JAVA** 

* Versatile client side programing language. (client side till node.js comes into the picture)
* Responds to events and can modify HTML on the go. 
* JS can be used for 
  * Form validation
  * Hide/show elements 
  * Dynamic web contents management
  * Event handling

#### Adding JS to web page 

1. Inside the `<scrip>` tag

    ```html
    <script>
    document.write("Hello World");
    </script>
    ```
2. Link external document (just like we did in CSS)
    ```html
    <script href="script.js"> </script>
    ```
#### Function Declaration. 

* Function without parameters. 
    ```JS
    function myFuntion {
        //do fun stuff here.
    }
    ```
* Function with parameters. 
    ```JS
    function myFuntion2 (para1,para2) {
        //do fun stuff here.
    }
    ```
* Sample functions 
    ```JS
    // Function declaration. 
    function square(x){
    return  x*x;
    }
    // Function Expression
    const square = function (x){return x*x}

    //Arrow Function expression.
    const square = (x) => {rerurn x*x}

    // Concise Function expression 
    const square = x => x*x ;
    ```
