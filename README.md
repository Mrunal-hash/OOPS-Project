WAR GAME

A simplified version of WAR GAME with two players.
Classes used:
1. Card: (card.py)
   returns suit and rank of the card
2. Deck: (deck.py)
   1. shuffle(): shuffles the deck of cards
   2. deal_one(): deal cards among the players
3. Player: (player.py)
   1. remove_one(): pops out a single card from the player to play
   2. add_cards(): add a card or list of cards to the player who wins war

GAME LOGIC
1. There are two instances of players
2. Instance of a new deck. Split half in between player 1 and 2
3. Loss check at the beginning: Check for 0 cards
4. Each player draw a card >> we compare
    1. If P1 > P2 = append both the cards in P1 at the bottom
    2. If P1 == P2 = Player draws additional 3 cards with
        while at_war loop. Once we get one player greater than the another
        it will append to the player with greater value
5. Check if player has 0 cards. If true, the opposite player has won
