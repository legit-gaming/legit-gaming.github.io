## Number Guessing Game - Project Step Instructions

#### **HTML**

##### Step 1 (START PROJECT HERE)
1. Create an HTML page with a header for now. When time allows, you can fancy it up!

##### Step 3 (Start with JavaScript Step 3)
1. Add a submit button.
2. Set the id attribute to submit
3. Add the onclick attribute and set it so that it triggers the guess function in your JavaScript file.

##### Step 7
1. Add a label to ask your user to enter a guess. 
2. Add a for attribute within the label tag and set it equal to the user's guess [e.g. for="inputGuess"]. 
3. Create an input field, with type="text" where the user can type in their guess. 
4. Set an id value for the input [e.g. inputGuess]. This is important so we can use/call this id value within our JavaScript file.
5. If you would like, also add placeholder text to hint to the user their guess should be betwen 0 and 100.
* **Note: The input will not be read just yet.

##### Step 9
1. Add a div tag wtih the following attributes, class="results", id="results". This tag should be added right before the closing body tag &lt;/body>.
2. Complete Step 9 in the JavaScript file

<br>

#### **JavaScript**

##### Step 1 (START WITH HTML Step 1)
1. Create a variable [such as var secretNum] to capture the secret number (computer generated number). For now, set this variable to any number between 0 and 100. 
2. Use an alert message to popup the secret number on the screen. 
3. Also display the secret number in the console. We'll use this to validate our code going forward. Run your program and see what happens!

##### Step 2
1. Create another variable to act as the 'player's guess' [such as var guessedNum] (for now) and set it to any number between 0 and 100. 
2. Define an if, else statement that will compare the secret number you defined in Step 1 to the player's guess and give hints to the user if their number is too high, too low, or correct!
3. Within each condition, use an alert to present the message to the player. 
4. Run your program and see what happens! Try running it multiple times, by setting your 'player's guess' variable to a number higher than the secret number, lower than the secret number, equal to the secret number.
* **Message e.g., if the player's guess is > the secret number, present a message 'Sorry, your guess was too high'

##### Step 3 (Complete JS Step 3 before HTML Step 3)
1. Wrap your if/else statement within a guess function [called something like checkMyGuess()].
2. Delete the alert from step 1, where you displayed the secret number. 
3. Move your console.log statement from Step 1 to the end of the guess funtion.
4. Flip over to your html file now (Step 3) to add a button that will call this guess function.

##### Step 4
1. Set your secret number variable at the top of your file to 0. 
2. Create a Random Number function [call it something like generateRandomNum()], above your guess function. 
3. Within the Random Number function, reset your secret number variable to a random number between 0 and 100. 
* **Make sure to call your function! 
4. Play the game multiple times and notice each time the secret number will change! To replay - click the refresh button next to preview in the display window to the right.

##### Step 5
1. Create a new variable (before of all the functions) [called something like var message], which will be a global variable at the top of your file , and set the value to an empty string "". This variable will store the messsage (too high, too low, etc.), that you will present to the user. 
2. Create a new function which we will use to trigger the message result you will present to the player [e.g. resultMessage()]. 
3. Inside the result message function, use an alert to display the message variable to the user, and also print your message variable along with the secret number [e.g. message + " " + secretNum] to the console. 
* **Note: This message will not print when you run your program because we are not calling the funtion anywhere...yet!

##### Step 6
1. Within your if/else conditions, remove the alert function and instead set your display message to your message variable which you created in step 5.
2. Before the end of your guess function, call your resultMessage function. 
3. Comment out the console.log statement within the guess function.

##### Step 7 - Flip over to your html file to create an input field to collect your users guess

##### Step 8
1. Set your user's guess number variable at the top of your file to 0.
2. At the top of your guess function, before the if statement, add a line of code to set the guess number variable [e.g. guessedNum] to the number input by the user. Hint: Use document.getElementById to do this.
3. Run your game by entering a guess into the input field and selecting the guess/submit button. Keep guessing until you are correct. Then reset the game by selecting the refresh arrow next to Preview in the display window to the right.

##### Step 9 - (Start with HTML step 9)
Let's now display the message to the user on the screen versus in the alert window
1. Start with step 9 in the html file

* Once your <div> tag has been added within the html, let's return the message to it.
2. Remove or comment out the alert from the results message function.
3. Within the result message function [e.g. resultMessage] create a new variable to hold the result [e.g. var results].
4. Set this variable to the id for your div, using document.getElementById
5. Add the following line of code below this variable    
* **results.innerHTML = "&lt;p>" + message + "&lt;/p>";**

* **Note: in the above line of code, results is the variable name you created in step 2. Message is the variable you created in step 5 to hold the message you share with the user.
* **The above line of code will add the HTML paragraph (made up of the message) to the location of the div tags on the HTML page.

##### Step 10 - Finally, let's track how many times it takes the user to guess the correct number.
1. Create a new global variable at the top of your file to capture the count of times a user guesses. [e.g. var count].
2. At the end of the generate random number function, set the count variable to 0. We do this again, so that when we play a new game and pick a new secret number, we also are sure to reset the counter back to 0.
3. At the top of the guess function, increase the count by 1. You can do this many ways, but two examples are using count++  or count = count + 1
4. Update the messaging within your if/else statement, so that when the correct number is guessed, the message displayed to the user also tells them how many tries it took them.
* **We put this in the guess function, because it is called every time we select the guess button to submit another try. Ultimately, this counter tracks the number of times we hit the button - or take a guess.

<br>

#### **Bonus Features**
* Allow the user to set the guess range. Right now we have the code defaulted to 100. Take input from the user to set that value. e.g. 20, 50, 200
* Make the messages back to the user more dynamic
  * Collect the user's name and print it in a response
  * If the user guesses an inccorect number, tell them how 'warm' or 'cold' they are based on how far away their guess is from the correct number.
* Add more styling to the page using CSS
  * Here are some Thimble Exercises you can work on and use as a guide - Choose Remix and follow the Tutorial Tab above the display screen:
    * [Keep Calm Poster - Good Way to Learn HTML and CSS](https://thimble.mozilla.org/en-US/user/legitliberty/1255829)
    * [CSS Building Blocks (How to Style a &lt;div> tag)](https://thimble.mozilla.org/en-US/user/legitliberty/1255775)
    * [HTML Burger - no Tutorial but a good chance to play around with CSS](https://thimble.mozilla.org/en-US/user/legitliberty/1255828)
