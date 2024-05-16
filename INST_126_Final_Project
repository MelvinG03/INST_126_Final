import random

class WordGuessingGame:
    def __init__(self, word_bank, theme, reveal_word_length=True, display_guessed_letters=True):
        self.word_bank = word_bank
        self.theme = theme
        self.reveal_word_length = reveal_word_length
        self.display_guessed_letters = display_guessed_letters

    def select_secret_word(self):
        return random.choice(self.word_bank)

    def play_game(self):
        secret_word = self.select_secret_word()
        if self.reveal_word_length:
            print(f"The secret word is related to {self.theme} and has {len(secret_word)} letters.")
        
        guessed_letters = []
        word_guesses = 0
        letter_guesses = 0

        while True:
            guess = input("Guess a letter or the whole word: ").lower()

            if len(guess) == 1:
                letter_guesses += 1
                guessed_letters.append(guess)
                occurrences = secret_word.count(guess)
                print(f"The letter '{guess}' occurs {occurrences} time(s) in the secret word.")
            else:
                word_guesses += 1
                if guess == secret_word:
                    print("Congratulations! You've guessed the secret word!")
                    break
                else:
                    print("Incorrect word guess.")

            if self.display_guessed_letters:
                print("Guessed letters:", guessed_letters)

            if word_guesses == 3:
                print("You've used all your word guesses. Game over.")
                break

        print(f"Total letter guesses: {letter_guesses}, Total word guesses: {word_guesses}")

# Example usage
word_bank = ["python", "programming", "computer", "algorithm", "variable"]
theme = "programming"

game = WordGuessingGame(word_bank, theme)
game.play_game()
