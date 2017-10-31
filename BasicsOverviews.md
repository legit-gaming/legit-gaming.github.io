## Understanding the Basics

1. Print with console.log
2. Create variables
3. Solve math problems
4. Use alerts
5. Use if statements
6. Create functions
7. Add buttons
8. Create a random number
9. Variable scope
10. Grab data from a webpage
11. Using &lt;div> tags

### 1. Print with console.log

JavaScript has a tool called console with a feature called log, which allows us to print messages.  This will be very helpful while we learn JavaScript to see what our code is doing.  Try adding the following examples into a JavaScript file within thimble, click run, and inspect the output.

```javascript
console.log('Code Girl: Game Makers');
console.log(4);
console.log(4.5);
```

The `console.log()` feature takes what we call parameters, such as text or numbers, and prints the provided input.  

[Try changing the inputs and look at the results.](https://legit-gaming.github.io/PracticeExercises.html)

### 2. Create Variables

Variables allow us to save data, so that we can use it multiple times.  With JavaScript we can create variables that hold text, numbers, and other items we will learn about later.  Let's take a look at how we can create and use variables from our last example.

```javascript
var course = 'Code Girl: Game Makers';
var favoriteNumber = 4;

console.log(course);
console.log(favoriteNumber);
```

To create a variable, we start off by saying `var` to tell JavaScript that we want a variable, then we give it a name.  Once we have a name, then we can set it equal to the value we want.  In the examples above we set a variable equal to some text and another variable equal to a number.  Instead of needing to type out the text or number again, we can now give `console.log()` our variables instead.  

[Try creating your own variables and printing them to console.](https://legit-gaming.github.io/PracticeExercises.html)

### 3. Solve math problems

We can use math operators, such as +, -, \*, and / with JavaScript to solve math problems.  Take a look at the examples below.

```javascript
console.log(2+2);
console.log(2*4);
console.log(9-5);
console.log(100/5);
```

We can also use variables and math operators together to solve problems.  Check out the examples below.

```javascript
var amountOfApples = 5;
var amountOfOranges = 8;
var amountOfGrapes = 30;

var amountOfFruit = amountOfApples + amountOfOranges + amountOfGrapes;
console.log(amountOfFruit);
```

[Try creating your own variables and math problems.](https://legit-gaming.github.io/PracticeExercises.html)

### 4. Use Alerts

The `alert()` function, will display text in a dialog box that pops up on the screen, sharing a message with the user. An alert box is often used if you want to make sure information comes through to the user.

```
alert("I am an alert box!");
```

The alert dialog should be used for messages which do not require any response on the part of the user, other than the acknowledgement of the message. When an alert box pops up, the user will have to click "OK" to proceed. 

Dialog boxes are modal windows - they prevent the user from accessing the rest of the program's interface until the dialog box is closed. For this reason, be careful and do not overuse the use of a dialog box (or modal window).

Alerts can also be triggered within a function:
```
 function showAlert() { 
   alert ("Hello world!");
  }
  showAlert();
```
[Try creating your own alerts and see what displays on the screen.](https://legit-gaming.github.io/PracticeExercises.html)

### 5. Use if statements

JavaScript to conditionally run code based on conditions we provide.  It provides a feature called if statements to help us with this.  Let's walk through an example.

```javascript
var numberOfApples = 5;
var numberOfPears = 8;

console.log('Does numberOfApples equal numberOfApples?');
if (numberOfApples === numberOfApples) {
  console.log('Yes!');
} else {
  console.log('No');
}

console.log('Does numberOfApples equal numberOfPears?');
if (numberOfApples === numberOfPears) {
  console.log('Yes!');
} else {
  console.log('No');
}

console.log('Does numberOfApples not equal numberOfPears?');
if (numberOfApples !== numberOfPears) {
  console.log('Yes!');
} else {
  console.log('No');
}

console.log('Is the numberOfApples greater than the numberOfPears?');
if (numberOfApples > numberOfPears) {
  console.log('Yes!');
} else {
  console.log('No');
}

console.log('Is the numberOfApples less than or equal to the numberOfPears?');
if (numberOfApples <= numberOfpears) {
  console.log('Yes!');
} else {
  console.log('No');
}
```

The conditions we place within the if statement returns a value of `true` or `false`.  If the condition is true, then it runs the code within the condition's block.  If a condition is false, then it will check the next condition until it finds one that is true.  Here are a couple other examples of if statements.

```javascript
var numberOfApples = 3;
var numberOfOranges = 9;

if (numberOfOranges > numberOfApples) {
  console.log('More oranges than apples');
}

if (numberOfOranges < numberOfApples) {
  console.log('This is false and will not get executed');
} else if (numberOfOranges > numberOfApples) {
  console.log('This is true and will execute');
} else {
  console.log('The previous condition passes, so we do not get to here');
}
```

[Try creating your own if statements.](https://legit-gaming.github.io/PracticeExercises.html)

### 6. Create functions

We have already used a couple functions, such as `console.log()`, `Math.random()`, and `Math.floor()`.  We can tell they are functions, because they end with parentheses.  Functions allow us to write some code, save it for later, and run it multiple times.  Let's create a function for generating a random number.

```javascript
function getRandomNumber() {
  var max = 10;
  var randomNumber = Math.random() * max;
  var noDecimalsRandomNumber = Math.floor(randomNumber);

  console.log(noDecimalsRandomNumber);
}

getRandomNumber();
getRandomNumber();
getRandomNumber();
```

We tell JavaScript that we want to create a function by saying `function` and then giving it a name with parentheses.  Once we have that settled, then we create some open and closing squiggly brackets with our code we want to save in the middle.  After we are finished creating our function, then we call it by name.

We can make our function a little more flexible by passing in parameters.  Say we do not always want 10 to be the max number, so we can tell our function what max we would like.

```javascript
function getRandomNumber(max) {
  var randomNumber = Math.random() * max;
  var noDecimalsRandomNumber = Math.floor(randomNumber);

  console.log(noDecimalsRandomNumber);
}

getRandomNumber(10);
getRandomNumber(50);
getRandomNumber(100);
```

Functions can also return things for us.  This can helpful if we want a function to do some work for us and provide us the result.  Let's take a look at some examples.

```javascript
function addNumbers(numberOne, numberTwo) {
  return numberOne + numberTwo;
}

var twoPlusTwo = addNumbers(2, 2);
console.log(twoPlusTwo);

function getRandomNumber(max) {
  var randomNumber = Math.random() * max;
  var noDecimalsRandomNumber = Math.floor(randomNumber);

  return noDecimalsRandomNumber;
}

var someNumber = getRandomNumber(15);
console.log(someNumber);
```

[Try creating your own functions and print the result.](https://legit-gaming.github.io/PracticeExercises.html)

### 7. Add buttons
We can try to make our webpage a little more interactive using buttons.  Buttons can be created in two ways: using the an input tag or button tag. 
 
Let's start with `<button>`

```html
<button>Click Me</button>
```
We can also add attributes to our button tag. For example, adding the id attribute will give a name to this button, making it unique, and also allowing it to be referenced by your JavaScript file if/when needed.

```html
<button id="buttonSubmit">Click Me</button>
```

How do we make our button run JavaScript when it is clicked?  We can use the onclick attribute!

```html
<button id="buttonSubmit" onclick="clickMe()">Click Me</button>
```

Now when the button is clicked it will run the `clickMe()` function in our Javascript.  However, we do not have a clickMe function, so let's write it.

```javascript
function clickMe() {
 console.log("Button clicked");
 }
```

As mentioned above, you can do the same thing with `<input>`. Take a look!
```html
<input id="inputSubmit" type="button" value="Click Me" onclick="clickMe()"/>
```
As you can see, it is very similar to `<button>`, but `<input>` has it's own specific attributes: type - which sets it as a button component on the page, value - name visible to the user on the button. Like `<button>`, `<input>` uses the onclick attribute to call the JavaScript function - in this case, `clickMe()` 

[Try creating your own buttons.](https://legit-gaming.github.io/PracticeExercises.html)

### 8. Create a random number

To create get a random number we can use the `Math.random()` feature.  It returns a decimal value between 0 and 1.

```javascript
console.log(Math.random());
```

However, what if we want a number between 0 and 10?  We can simply multiply our random value with 10.

```javascript
var max = 10;
var randomNumber = Math.random() * max;

console.log(randomNumber);
```

We might not want those decimals on our random number, so we can use `Math.floor()` to chop them off.

```javascript
var max = 10;
var randomNumber = Math.random() * max;
var noDecimalsRandomNumber = Math.floor(randomNumber);

console.log(noDecimalsRandomNumber);
```

[Now try creating your own random numbers.](https://legit-gaming.github.io/PracticeExercises.html)

### 9. Variable Scope
JavaScript variables have "function scope". A variable can have **local** or **global** scope. 

Scope determines the accessibility (visibility) of these variables and can be determined based on the location or placement of the variables within your code. 

For example, a variable defined inside a function is not accessible (visible) from outside the function. It becomes **LOCAL** to that function.

Here's an example of a variable with **LOCAL** scope:

```
//code here cannot use color

function favColor(){
  var color = "blue";
  //code here can use color
  console.log("My favorite color is " + color);
  //code here can use color
}

//code here cannot use color
```
As you can see in the above example, we created a new variable called 'color' within the function. Since it is local, it means that the variable belongs to the function and is not visible or cannot be accessed by any other code outside that function. 

For example, in the following code, the alert outside of the function would receive an error when trying to print - because it doesn't recognize the color variable.

```
function favColor(){
  var color = "blue";
  console.log("My favorite color is " + color);
}

alert(color);
```

Local variables are created when a function starts, and deleted when the function is completed. Since local variables are only recognized inside their functions, variables with the same name can be used in different functions.
For example:

```
function favColor(){
  var color = "blue";
  console.log("My favorite color is " + color);
}

function secondFavColor(){
   var color = "black"'
   console.log("My second favorite color is " + color);
}
```


A variable with **GLOBAL** scope, is declared outside a function and can be accessed anywhere throughout your code.

var color = " ";

```
function favColor(){
  color = "blue";
}

alert("My favorite color is " + color);
```

In the above example, both the function and the alert would successfully read and use the color variable.

[Now, try playing around with locally and globally scoped variables.](https://legit-gaming.github.io/PracticeExercises.html)

### 10. Grab data from a webpage 

Let's start off by creating an input box on webpage.  We can do this by adding the following element to our html page.

```html
<input type="text" id="myInput" />
```

Now if someone types something into our textbox how could our JavaScript grab that information?  We can inspect the document object model (DOM).  When a webpage loads it builds a document object, which creates a number of children objects that represent the items we wrote in our HTML.  For example, the input we wrote above is a child of our document.  Now let's walk through how we can grab the value of the input box with JavaScript.

```javascript
var myInput = document.getElementById('myInput');
var myInputValue = myInput.value;

console.log('myInput Value: ' + myInputValue);
```

On the first line, we use the `document` object, which is globally available.  This means JavaScript can always access it.  We then tell the document object we want to grab one of its children, also called an element in this case, by their id.  We do this by calling the `getElementById` function and providing it the id of our textbox.  It returns the textbox object, which we can grab the value from by saying `myInput.value`.

```javascript
function clickMe() {
 var myInput = document.getElementById('myInput');
 var myInputValue = myInput.value;
console.log('myInput Value: ' + myInputValue);
}
```
    
We took the code we wrote from earlier, so now when we click the button it will print the value of the text box to console.  We can then use an alert so that users can view the value on the screen instead of the console.

```javascript
function clickMe() {
 var myInput = document.getElementById('myInput');
 var myInputValue = myInput.value;
 alert('myInput Value: ' + myInputValue);
}
```

[Try this out!](https://legit-gaming.github.io/PracticeExercises.html)

### 11. Using &lt;div> tags

A `<div>` tag is used to group a section of your html content together. It groups a block of elements/tags (such as a `<p>`, `<img>`), which can make it easier to organize and style your webpage with css.

Let's start with sharing formatting. In the following example, all elements within the div tag will be styled with the color green.

```html
<div style="color:green">
  <h2> This header will be the color green. </h2>
  <p> All of the text within these paragraph tags will be green. </p>
</div>
```

A div tag can hold both an 'id' and 'class' attribute, which allows us to identify this section of content. 

A 'class' attribute with the same name can be used on multiple elements on our webpage and we can use this to style multiple elements in the same way. 

The 'id' attribute must have a unique name and that name can only be used on one element on your webpage.  We can also use JavaScript to grab an element by its unique id.

Take a look at the following HTML, CSS, and JavaScript files:

**CSS**
```css
.paragraph2 {
  color: blue;
}
```

**HTML**
```html
<html>
<head>
<script type="text/javascript"></script>
</head>

<body>
  <p> This is paragraph 1 </p>
  
  <div id="paragraph2" class="paragraph2"></div>
</body>

</html>
```

**JavaScript**

Example 1:
```javascript
document.getElementById("paragraph2").innerHTML = "This is paragraph 2";
```

Example 2:
```javascript
var content = document.getElementById("paragraph2");    
content.innerHTML = '<p>' + "This is paragraph 2" + '</p>';
```

[Take a shot on your own!](https://legit-gaming.github.io/PracticeExercises.html)
