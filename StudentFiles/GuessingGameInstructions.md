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


**JavaScript**

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
