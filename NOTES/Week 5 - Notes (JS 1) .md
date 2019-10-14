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
#### Variable Declaration

Two types of variable declaration 
*global* : variables declared outside the function
*local* : variables declared inside the 
Do datatype required. 
sample var declaraion
```js
var myName  = "Qasim";
var myID = 42;
//and so on
```
#### String type var
Strings in JS are enclosed in double or single quotes
```js
var a = "Qasim";
var b = "42";
var c = '42';
//to add quotes in the string use different quote from that of container 
var d = "this is the 'message' in quotes";
//add stings together using +
var e = "Hello" + a + "I like" + b ;//Hello Qasim I like 42
```
#### Number datatype
Js has only one Number type can cannot be written with decimal
```js
var f = 42;
var g = 42.00;
var h = 42e7; //420000000
var i = 42e-7; .0000042

```
#### Boolean 
either trur or false 
```js
var isANum = false;
var isAbool = true;
```
#### Arithmetic operations. 
let a = 10; 
```Js
//Increment
b = a++; //b=10 a=11
b = ++a; //b=11 a=11
//Decrement 
b = a--; //b = 10 a =9
b = --a; //b = 9 a = 9
```
#### Assignment operators 
let a = 10 b = 5 
```js 
// a = a + b 
a += b // a = 15 b= 5
a -= b // a = a - b a = 5
a *= b // a = a * b a = 50
a /= b // a = a/b a = 2
a %= b // a = a%b a=0 "Mod is the reminder."
```
#### comparison operators 

let a = 10 

```js
(equals) == vs === (exactly equal)
== checks for value, === checks for value and datatype. 

&& and 
|| or 
! not
```

#### conditional statements 

```js

//IF ELSE IF
if (boolean_expression){
    //if true.
    doSomething();
} else if (someOtherBool_expression){
    doSomeThingElse();
} else {
    doThisIfNoneAbove();
}

//SWITCH
switch  (variable) {

    case 1: //value after case is called label ..if label matches variable 
        //do this 
        break; // tells the switch to stop. 
    case 2: 
        //else do this
        break;
    default:
        //if none above do this. 
} 
```
#### Alert and Prompt

Alert sends a warning message to the user. 
```js
alert ("please enter a value");
```
prompts display message bos that take a value from the user.
the results of the user input can be assigned to a variable for example. 
```js
var name = prompt ("What is your name ?", "Joker") // asking user with default value. 
```

### HTML and JS interaction. 

There are attributes in HTML that can run JS when a certain event happens.

Some attributes are 
    - onclick
    - onmouseover
    - onload
    - onchange
    - onmouseup
    - onmousedown
These attributes can be used to triger a JS function. for example. 

```HTML
<script> 
function say_hello(){
    var user_name = prompt ("What is your name?", "Joker");
    alert("Hello " + user_name);
}
</script>
<input type = "button" name="hello_btn" value="click me" id="hello_btn" onlclick="say_hello();">
