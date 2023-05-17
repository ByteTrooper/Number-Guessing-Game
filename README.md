# Number-Guessing-Game
'''
Here's a step-by-step breakdown of the code:

The HTML file begins with the <!DOCTYPE html> declaration, indicating that this is an HTML5 document.

The <head> section contains the <title> element, which sets the title of the web page displayed in the browser's title bar.

The body section contains the game elements:

The h1 element displays the heading "Number Guessing Game" at the top of the page.

The p element displays the prompt message "Guess a number between 1 and 10:" to instruct the player.

The input element with the type attribute set to "number" creates an input field where the player can enter their guess. The id attribute is set to "guessInput" to uniquely identify the input field.

The button element displays the "Guess" button. The onclick attribute is set to the JavaScript function checkGuess(), which will be called when the button is clicked.

The p element with the id attribute set to "result" is initially empty. It will be used to display the result of the player's guess.

The script section contains the JavaScript code:

The first line generates a random number between 1 and 10 using Math.random(). The Math.floor() function is used to round the result down to the nearest whole number. The generated number is stored in the randomNumber variable.

The checkGuess() function is defined. This function is called when the player clicks the "Guess" button. It retrieves the player's guess from the input field using document.getElementById('guessInput').value. The parseInt() function is used to convert the input value from a string to an integer.

Inside the checkGuess() function, an if statement is used to compare the player's guess with the randomly generated number:

If the guess is equal to the randomNumber, a success message is displayed by setting the textContent property of the p element with the id of "result".

If the guess is less than the randomNumber, the code block inside the else if statement is executed. It sets the textContent property of the p element with the id of "result" to display the message "Too low. Try again!".

If neither of the above conditions are met, it means the guess is greater than the randomNumber. The code block inside the else statement is executed, setting the textContent property of the p element with the id of "result" to display the message "Too high. Try again!".

After defining the checkGuess() function, the script section ends.

In summary, the HTML code creates a simple number guessing game interface with a heading, prompt message, input field, and a button. The JavaScript code generates a random number and compares the player's guess with it to provide feedback. The result is displayed in a paragraph element on the web page.


'''





