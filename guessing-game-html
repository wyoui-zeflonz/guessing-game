<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Number Guessing Game</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }
    </style>
</head>
<body>
    <h1>Number Guessing Game</h1>
    <p>Guess a number between 1 and 100:</p>
    <input type="number" id="guessInput">
    <button onclick="checkGuess()">Guess</button>
    <p id="message"></p>

    <script>
        // Generate a random number between 1 and 100
        const randomNumber = Math.floor(Math.random() * 100) + 1;

        // Function to check the user's guess
        function checkGuess() {
            const guess = parseInt(document.getElementById('guessInput').value);
            const messageElement = document.getElementById('message');
            
            if (isNaN(guess) || guess < 1 || guess > 100) {
                messageElement.textContent = 'Please enter a valid number between 1 and 100.';
            } else if (guess === randomNumber) {
                messageElement.textContent = 'Congratulations! You guessed the correct number!';
            } else if (guess < randomNumber) {
                messageElement.textContent = 'Too low! Try a higher number.';
            } else {
                messageElement.textContent = 'Too high! Try a lower number.';
            }
        }
    </script>
</body>
</html>
