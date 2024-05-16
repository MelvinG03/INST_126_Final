# INST126_FinalProject

1. Define a class WordGuessingGame:
Initialize the class with the word bank, theme, reveal_word_length, and display_guessed_letters options.
Define a method select_secret_word() to randomly select a word from the word bank.
Define a method play_game():
Select a secret word using select_secret_word() method.
If reveal_word_length is True, display the length of the secret word and its theme.
Initialize an empty list to store guessed letters.
 Initialize variables for word_guesses and letter_guesses to track player's guesses.
Start a loop:
Ask the player to guess a letter or the whole word.
If the guess is a single letter:
Increment letter_guesses counter.
Add the guessed letter to the guessed_letters list.
Count occurrences of the guessed letter in the secret word.
Display the number of occurrences of the guessed letter in the secret word.
If the guess is the whole word:
Increment word_guesses counter.
Check if the guess matches the secret word:
If correct, display a congratulatory message and end the game.
If incorrect, display an incorrect message.
If display_guessed_letters is True, display the guessed letters list.
Check if the player has used all their word guesses:
If yes, display a game over message and end the game.
Display the total number of letter guesses and word guesses made by the player.
2. Create an instance of the WordGuessingGame class with a word bank and theme.
3. Call the play_game() method to start the game.
