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
<input type = "button" name="hello_btn" value="click me" id="hello_btn" onclick="say_hello();">
```

### Document Object Model 
*  DOM is web programing acts as a link between programing and we pages. 
*  HTML element are treated as objects 
*  DOM contains all the elements of the page when loaded into the browser.
*  HTML 
   *  elements
   *  attributes
   *  comments 
are all sub nodes of the document object they exists in. 

#### Some Key DOM properties 
  * document.cookie  - Returns the document's cookie
  * document.images - Returns all ```<img>``` elements
  * document.title - Returns the ```<title>``` element
  * document.URL - 	Returns the complete URL of the document
  * document.anchors -	Returns all ```<a>``` elements that have a name attribute
  * document.forms -	Returns all ```<form>``` elements

#### Some Key DOM Methods
  * document.getElementById("Qasim")  - Returns the element with the id "Qasim"
  * document.write("Qasim") - Writes "Qasim" into output. 
  * document.getElementByTagName("LI") - Get all elements in the document with the specified tag name "LI"
  * document.createElement()- 	Returns the complete URL of the document
```js
var btn = document.createElement("BUTTON");
  btn.innerHTML= "Qasim";
  btn.id = "Qasimbtn";
```
 *  All types of elements have shared properties and methods for example 
>element.childNodes
will return  all the nodesList contains child nodes. can be accessed using element.childnode[3]
* Node list contains list of all child nodes can be looped using for loop.
  
#### key element object properties. 
  * element.attributes - Returns all attribute nodes registered to the specified node
  * element.id - sets or returns the id of the element. 
  * document.innerHTML - sets or returns the contents of the element. 
  * document.className - sets or returns the contents of the element. useful in applying css style dynamically. 
  #### key element object Methods 
  * element.setAttribute() - Returns all attribute nodes registered to the specified node
    * >element.setAttribute("style", "background-color: red;");
  * element.clodeNode() -Clones an element 
    * >var cln = itm.cloneNode(true);
  * element.appendChild() - appends a new node before specified child. 
    * > document.getElementById("myList1").appendChild(cln); 
  * document.removeChild - removes a specific child node.
    * > document.getElementById("myList1").removeChild(cln); 

#### The attribute object

* used to edit HTML attributes
* attributes are returned in a namedNodeList. 
* namedNodeList can access attributes by index or by name. 
  * element.attribute.name - returns the name of att
  * attribute.value - sets or returns the value of att 
  * attribute.specified - returns true if the attribute is specified.

### Events
* registers events.
  * Mosue events
    * onclick
    * onmouseup
    * onmousedown
  * Fram/object events
    * onload 
    * onerror
    * onabort
  * foram event 
    * onchange
    * onfocus
    * onsubmit
* usually used in conjunction with a function. 
  * > document.forms[“myForm”].onsubmit= validateForm();will call the validateForm() method when the form is submitted.


#### The input text object. 

* some elements have their own objects (attributes)
* for example input text element has 
  * properties like
    * value - returns or sets teh value of text box 
    * maxlength - returns or sets the size of textbox in characters 
    * size - returns sixe of the textbox. 
  * Methods 
    * select () - slects the size of the textbox. 
* The input radio/checkbox 
  * properties 
    * checked - returns or sets bool value. 
    * value - returns or sets the value.
#### Javascript Arrays
*   multiple values in one object. 
    * Properties 
      * length
    * methods
      * sort()
      * push() - adds a new element onto the end of array
      * concat() -  joins two arrays
    * Constructor
      * > var newArray = new Array();
    * literal 
      * > var newArray = ["item1", "item2"];
    * condensed  
      * var newArray = new Array("item1", "item2");
