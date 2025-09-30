# Best-Poker-Hand-Game
"A Python poker game that evaluates hands, identifies the best possible hand from community cards, and compares player input to the optimal hand. Uses OOP, combinatorics, Counter, sorting, and threading to implement hand detection, ranking, and timed gameplay with normal and hard modes."

Poker Hand Game

This project is a Python-based poker game that simulates evaluating and comparing poker hands in a user-interactive environment. The game presents players with a set of five community cards and challenges them to determine the best possible hand by guessing two additional cards. The AI concurrently calculates the optimal hand from the same deck, allowing players to compete against a computer opponent. The game supports both normal and hard modes, with hard mode introducing a dynamic countdown timer to increase difficulty.

The program is built using object-oriented principles with a Card class representing individual cards, encapsulating rank and suit information, and providing methods for comparison, hashing, and string representation. The full 52-card deck is generated programmatically, and cards are drawn randomly without replacement. Card input from the player is validated against rank and suit mappings, ensuring robustness against invalid or duplicate entries.

Hand evaluation is implemented using combinatorial logic and Python’s collections.Counter to detect pairs, two pairs, three-of-a-kinds, straights, flushes, full houses, quads, and straight flushes. Each hand is assigned a strength and tie-breaking value according to standard poker hierarchy, and evaluation functions return both the hand’s composition and descriptive name. Sorting algorithms ensure cards are ordered correctly for comparison, and reverse sorting is used for high-card and flush evaluation.

The game also incorporates threading to manage timers in hard mode, providing real-time feedback and creating a sense of urgency. Players interact with the game through a text-based interface, entering card guesses in a human-readable format (e.g., "Two of Spades"). The game loops through rounds until either the player or AI reaches the winning score, dynamically updating scores and displaying both player-created hands and the AI’s best hand for comparison.

Additional features include fast mode to accelerate gameplay, clear console output for readability, and modular functions that separate game logic, hand detection, and user interaction. The project highlights the use of object-oriented design, combinatorial search, sorting, mapping, and multithreading, demonstrating both Python programming techniques and algorithmic reasoning in the context of classic card games.
