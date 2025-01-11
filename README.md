# Playing-Cards

This project is a Java-based simulation of a standard deck of playing cards. It implements features like shuffling, sorting, drawing cards, and managing deck size, showcasing object-oriented programming principles.

---

## Features

### 1. **Card Representation**
- Each card has:
  - **Suit**: Spade, Club, Heart, or Diamond.
  - **Rank**: Ace, Jack, Queen, King, 2-10.
  - **Color**: Cards are classified as either Red (Hearts, Diamonds) or Black (Spades, Clubs).

### 2. **Deck Operations**
- **Shuffle**: Randomly rearranges cards in the deck using the `Collections.shuffle` method.
- **Draw a Card**: Removes the top card from the deck and returns it. Throws an exception if the deck is empty.
- **Sort**: Orders the deck based on the color, suit, and rank using a custom comparator.
- **Size**: Returns the current number of cards in the deck.

### 3. **Code Design**
- Implements enums for `Suit`, `Rank`, and `Color`.
- Uses a `Card` class to represent individual cards.
- A `Deck` class encapsulates all operations on the deck, including shuffling, sorting, and drawing cards.
- A nested `CardCom` class serves as a custom comparator for sorting cards.

---

## Code Overview

### Enums
1. **`Suit`**: Represents the suit of a card (Spade, Club, Heart, Diamond).
2. **`Rank`**: Represents the rank of a card (Ace, Jack, Queen, King, and numerical ranks).
3. **`Color`**: Represents the color of a card (Red for Hearts/Diamonds, Black for Spades/Clubs).

### Classes
1. **`Card`**:
   - Represents a single card with a suit, rank, and color.
   - Includes:
     - Getters for suit, rank, and color.
     - A `toString()` method for card representation.

2. **`Deck`**:
   - Contains a list of `Card` objects.
   - Provides methods for:
     - `Shuffle`: Randomizes the deck.
     - `DrawCard`: Draws a card from the top.
     - `Sort`: Sorts cards by color, suit, and rank.
     - `Size`: Returns the number of cards left in the deck.
   - Includes a nested `CardCom` class to compare cards for sorting.

3. **`PalyingCards`**:
   - Main class with a `main` method to demonstrate deck operations.

---

## How to Run

### Prerequisites
- Java Development Kit (JDK) installed.

### Steps
1. Compile the code:
   ```bash
   javac PalyingCards.java
2. Run the program:
java PalyingCards
3. Sample Output
Here's an example of how the program behaves:
Deck{ c= [A of Spade, J of Spade, Q of Spade, K of Spade, two of Spade, ...]}
Size is 52
Size is 51
Deck{ c= [six of Heart, eight of Diamond, ...]}
Size is 50
Card drawn is three of Club
### Future Enhancements
* Add functionality for multiple decks.
* Extend support for additional card games.
* Include a user-friendly GUI to visualize the deck and gameplay.


