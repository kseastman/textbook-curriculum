# Object Oriented Design Practice

The purpose of this exercise is to give you practice designing objects and the way they would interact. The goal is _not_ to write the code to complete the exercise, though you're welcome to if you would like. There aren't right or wrong answers, specifically, but _decisions_ you can make to structure your code.

## Problem Statement
We need to design a system that would allow us to utilize a deck of cards in a [BlackJack game](https://www.youtube.com/watch?v=qd5oc9hLrXg). This deck and cards should not have behavior specific to any particular game, while a Game class would relate to the specific implementation of BlackJack.

The user of a deck of cards should be able to shuffle the cards as well as deal cards. To deal, the user should be able to specify the number of players who will be dealt a specified number of cards.

## Design
|Questions:| |
|:---------|:---------------|
|How does a deck relate to a Game?| It is a separate class that the class Game will call upon to initialize |
|How does a card relate to a deck?| A card is an object created by a factory by suit, that the deck calls upon to initialize a deck object|
|What properties would a Game have?| A game would have the game logic for the game, it would have a method to deal cards, to add the value of specific cards, to let the user hit for an additional card, and to make the dealer hit if it is below a certain value and stay if it is over that value, as well as determine the win condition based on whether the hand went over or was higher|
|What properties does a card have?| a suit and a numerical value (Jack - Ace have pictures -- maybe ascii -- in addition to values) |


## Complete
- Determine which classes you would create
  - For each class, define the attributes and methods you would utilize
  - Method definitions should include any parameters you would be using as well as return values

| Class | Attributes | Methods|
|:----:|:------:|:------:|
|Card| @face, @points, @suit | #self.new(hearts, spades, clubs, diamonds) return 13 cards per suit, 2 - Ace |
|Deck| @cards | #shuffle(times) : return randomized deck|
|Game| @deck @dealer @player | #deal(num_of_players) - includes dealer, #score(hand): return top score, |
|Dealer| @hand @money | #deal(card): return 2 top cards #deal_hit(deal): return 1 top card, #hit(deal) return self.1 top card, #stay: return - current hand for scoring|  
|Player| @hand @money | #hit(deal), #stay: return - current hand for scoring, #split(hand): return current hand split to two hands, deal 1 top card, #bet(wager): return float, #win(bet): return increment total money|
