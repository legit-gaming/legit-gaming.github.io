## Code Girl: Game Makers

Creating games with JavaScript

### Week 1

* Activity/Introduction/Nametags
* Set program ground rules - mentors to add to this website

* [HTML Overview/Refresh](HtmlRefresh.md)
* [What is JavaScript?](WhatIsJavaScript.md)
* Set scope for 7 weeks / explain Curriculum
* Thimble setup (creating blank JS file using green add button (remove pre-existing js function)  -- USE CHROME
* Walk through adding <Script> tag to html file
* Rename HTML file to number guessing game - 5 minutes to make it fun

* Paperwork - initial survey, photo release form
* Collect namecards
* Group Selfie
* Properly shutdown computers

* Number Guessing Game
Start with Number Guessing Game

Mentor Edition - Contains all solutions - Use legitLiberty account
[Game Makers: Week 1 Goals](https://thimble.mozilla.org/en-US/user/legitliberty/1186702/)

Before variables - run cup activity
Goal 1 (in JS file): Set variable to a hard coded number and print number to console
  * Intro to variables and types (for each - a page with description and examples - students to reference, thimble with example problems to solve (for mentors to use during live demons), thimble with solutions (for mentors only))
  * Introduce console.log
  
 Goal 2 (in JS file): Use +, -, \*, / to solve math problems -- utilize varibales as well
  * Simple arithmetic problems
  
 Goal 3 (in JS file): Set a variable to a random number and print it to the console
  * Intro to random number command

 Goal 4 (in JS file): Use a function to print a number, one that doubles their number or multiplies or sums them
  * Intro to functions and parameters
  * Explain returns - hold off initially?
  * Revisit Random command
  
 Goal 5 if statements
  * If/else statement with simple boolean
  * if/if-else/else statement
  * Greater/Less than boolean expression

[Week 1 Goals Walkthrough](./week1/Goals.md)

### Week 2

* Activity to breakup the class - can be done at the beginning, middle, end of the class (ice breaker or CS Unplugged)
  \*e.g. Bring in Pis with Minecraft one week, Lightbot

* Number Guessing Game
  * Review last week and answer any questions
  * Create html page with a text box for taking guesses and a submit button for checking the guess
  * Add script tag in html page to load JavaScript from last week
  * Create a checkGuess() function, which alerts the user of their guess when clicking the submit button
  * Create a function that generates and saves a random number

* Collect namecards
* Group Selfie
* Properly shutdown computers

### Week 3

* Activity/Nametags

* Number Guessing Game
  * Review last week and answer any questions
  * Update checkGuess() to see if the user guessed correctly and update the alert box to tell the user if they're correct
  * Update the webpage with a message, rather than use an alert box 
  * Add more boolean conditions in checkGuess() to tell the user if they're getting closer to the secret number

* Collect namecards
* Group Selfie
* Properly shutdown computers

### Week 4

* Activity/Nametags

* Target Practice 
  * Introduce [p5](https://p5js.org/reference/) and [canvas](https://www.w3schools.com/graphics/canvas_intro.asp)
  * Setup HTML page with script tag for loading p5 and to JavaScript for the game
  * Introduce p5 setup lifecycle function
  * Create a canvas and draw shapes
    * Use different sizes, colors, strokes, etc.
  * Introduce p5 draw lifecycle function
    * Write drawTargets(), which draws a number of shapes

* Collect namecards
* Group Selfie
* Properly shutdown computers

### Week 5

* Activity/Nametags

* Target Practice 
  * Review last week and answer any questions
  * Introduce objects and arrays 
  * Write createTarget(), which returns a shape object with an x coordinate, y coordinate, and size
  * Write addTarget(), which calls createTarget every 30 frames and adds the target to the targets array

* Collect namecards
* Group Selfie
* Properly shutdown computers

### Week 6

* Activity/Nametags

* Target Practice 
  * Review last week and answer any questions
  * Introduce for loops
  * Update drawTargets() to loop through the targets array and draw the targets
  * Write growTargets(), which loops through the targets array and increases their size

* Collect namecards
* Group Selfie
* Properly shutdown computers

### Week 7

* Activity/Nametags

* Target Practice 
  * Review last week and answer any questions
  * Introduce mouse events and p5 mousePressed() function
  * Write mousePressed() function, loop through targets array and mark targets as hit when clicked
    * Check if mouseX and mouseY are in the location of a target
    * Add new attribute to target
  * Update drawTargets() to not draw circles that have been hit

* Collect namecards
* Group Selfie
* Properly shutdown computers
