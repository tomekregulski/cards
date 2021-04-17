## Cards

## Description

This project is part of Stephen Grider's course on Elixir and Phoenix, which I am currently taking and coding along. I have created a repo for it, solely for the purpose of my own learning as I approach a new programming language. I do not present this as my own work, though I may modify it as I gain comfort in working with Elixir.

This is a simple add that introduces the basic features of Elixir through the conept of a deck of cards. It features functions that build a new deck, check if a specific card is in the deck, shuffle the deck, deal a new hand, and write/read the data to/from a file.

## Installation

Clone this repository to a local directory, and ensure that you have the latest versions of Elixir via https://elixir-lang.org.

Then, open the directory in your terminal and install the necessary dependencies by running:

```
mix deps.get
```

## Use

Once the installations have completed, you are ready to run the app. Initiate the shell by running:

```
iex -S mix
```

The following lines of code will allow you to take avatnage of this program's functionality. Alternatively, this can all be accessed via the documentation, which can be accessed by first running the following command in the root directory:

```
mix docs
```

followed by:

```
open docs/index.html
```

To use this program, you must first create the deck of cards, which is done by running:

```
Cards.create_deck
```

You can shuffle the deck by running:

```
Cards.shuffle
```

You can check if the deck contains a specific card by running i.e.:

```
Cards.contains?(deck, Ace of Spades)
```

or

```
Cards.contains?(deck, Eight of Hearts)
```

You can deal a hand by running the following command, where hand_size is an integer i.e.:

```
Cards.deal(deck, hand_size)
```

The deck can be saved to a file by running:

```
Cards.save(deck, filename)
```

The file can be subsequently loaded by running:

```
Cards.load(filename)
```

Finally, you can create the deck, shuffle and deal a hand all at once by running i.e:

```
deck = Cards.create_deck
{ hand, _deck } = Cards.create_hand(Integer_Size_of_Hand)
hand
["King of Spades", "Jack of Hearts", "Four of Hearts", "Five of Diamonds",
"Queen of Spades"]
```
