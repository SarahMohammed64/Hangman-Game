
## 🎮 Hangman Game with Random Word API (Python)

This is a console-based implementation of the classic **Hangman** game in Python. It features a dynamic word selection system that fetches a random word from an online API, making each game unique. In case of network issues, it falls back to a built-in list of default words.

---

### ✅ Key Features

* 🔤 **Random Word Fetching**: Uses the [Random Word API](https://random-word-api.herokuapp.com/) to retrieve a new word each game session.
* 💡 **Fallback Mechanism**: If the API request fails, the game picks a word from a local predefined list.
* ⌛ **Limited Attempts**: Players have 6 tries to guess the word before the game ends.
* 🔁 **Interactive Gameplay**: Tracks guessed letters and prevents repeat inputs.
* 📄 **Clean Word Display**: Shows blanks (`_`) for unguessed letters and reveals correct guesses in-place.

---

### 🧠 How It Works

1. A word is selected either from the API or from a fallback list.
2. The player is prompted to guess one letter at a time.
3. Incorrect guesses reduce the remaining attempts.
4. The game ends when:

   * The word is guessed correctly, or
   * All 6 attempts are used

---

### 📝 Sample Gameplay

```
Welcome to Hangman!

_ _ _ _ _
You have already used the letters set()
Guess a letter: a

Incorrect! You have 5 attempts left.

_ _ _ _ _
You have already used the letters {'a'}
...
Congratulations! You guessed the word: hangman
```

---

### 🛠️ Tech Stack

* **Language**: Python 3
* **Libraries**:

  * `requests` – for HTTP requests to the random word API
  * `random` – to select a fallback word

---

### 🚀 How to Run

1. Ensure you have Python 3 installed.

2. Install the `requests` library (if not already installed):

   ```bash
   pip install requests
   ```

3. Run the game:

   ```bash
   python hangman.py
   ```
