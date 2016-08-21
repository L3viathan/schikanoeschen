# Schikanöschen

Schikanöschen is a game played by 2 opposing players.


##Goal
The goal of the game is to get rid of all cards on your side, and have all your
cards in the middle turned face-up.

##Setup
The game is played with Patience cards, i.e. two full card decks (52 cards + 3 jokers).
The two decks should be distinguishable by their backs, and are ideally half-sized
bridge or poker cards.

Two players sit on opposite ends of a table, facing each other.

To start, shuffle both decks thouroughly (one shuffled by each player), have each
player cut the deck of their opponent and then take their deck in their hands.

![Illustration of the initial setup and labels of the stacks](schikanoeschen.png)

Both player then deal 13 cards face-down on a stack, this stack is placed on their
side towards the right (stack C).

Using the remaining cards, the players then deal four cards seperately, vertically,
in the middle towards the right (stacks E-H). A face-up card is placed on the top-most
stack (stack E), and one face-down card each on the other three. Now a face-up
card is placed on the next stack (stack F) and a face-down card each on the other
two. This process is repeated until each stack has a face-up card and one to four
face-down cards (see illustration).
These stacks are arranged such that all cards are permanently visible, all other
stacks are neatly squared such that only the top card is visible.

Stacks E-H of both sides are considered the board, stacks D are the →final stacks,
stacks A-C are considered stacks of the player sitting in front of them.

The remaining cards become the main stack (stack A). The top card on stack C is
then turned around and the player with the higher card begins as the active player.
An ace is considered higher than other normal cards, a joker is higher than an ace.
If the two values are the same, then clubs is better than spades is better than
hearts is better than diamonds.

If the two cards are identical, the cards on stack E decide, and if those are
identical two, stack F, G, and H, in that order. If all open cards are exactly
the same, start over with shuffling.

##A Turn/States
At all times, one player is the active player and the other player is the passive
player. The only thing the passive player can do is knock (→Knocking).

The active player can move cards from one of her stacks (A, B, or C) and from the
board to the board, to the →final stacks, and to stacks B and C of the passive
player.

The active player can never take cards from the stacks A-C of the passive player.

If the active player takes a card from stack A and there's no other place to put
it (or if she chooses not to put it somewhere else), the card is put face-up on
stack B. This ends her turn, makes the other player the active player and her the
passive one.

Whenever the player wants to turn around a card from stack A, but it is empty
(but stack B is not), she turns around stack B, turning it into a new stack A,
and leaving stack B empty. This has to be immediately followed by taking and turning
around the top card of stack A; it is a single action. The stack is not shuffled.

##Moving cards
On the board, cards can be put on empty slots, on a face-down card. A card can
also be placed on a face-up stack card if the following three conditions apply:

- The card being placed is of a different color (red vs. black) than the stack
card
- The card has a value one lower than the stack card (e.g. two of diamonds on a 3 of spades)
- There is either no face-down card in the stack, or the amount of face-up cards
is no more than four after the card would have been placed down.

Cards can be moved on opponent stacks (B and C) if the stack card is one lower or
one higher than the card that is being placed, and they have the same suit.

Whenever a player moves the last face-up card from her stack C, the top-card has
to be turned face-up. This turning of the top card of stack C is a non-action and
can be done at any time legally (i.e. the passive player can never knock because
of it).

##Final stacks
The stacks in the middle are called "final stacks", because any card that has
been placed there will stay there indefinitely. Whenever an ace can be moved, it
has to be moved to one of the (empty) final stacks. When the next-highest card
is movable (the corresponding two), it has to be moved on the final stack, and so
on. Whenever a card can be moved to a final stack, it has to be done, and no other
actions may be done.

Cards from the board have priority over player stacks, i.e. if there are two cards
that have to be moved to a final stack, one on the board, and one on stack B or C
of a player, the one on the board has to be moved (first).

##Knocking
The passive player can choose to knock on the table in one of three cases:

- an active player would have to move a card to a final stack, but attempts
another move (by merely touching another card)
- an active player would have to move a card to a final stack, but attempts to
place it somewhere else (by placing it and ceasing to touch the card)
- an active player tries to place a card from her stacks B or C to a final stack,
but a card from the board could be moved to a final stack (by merely touching
her card)

The passive player can knock or choose not to knock. In the first case, the passive
player can also wait until the active player has made the (wrong) move and then
immediately knock. In that case and in the second case, the knocking player can
choose whether or whether not to revert the move.

The right to knock expires after another (legal) action has been done, even if
that action is the correction of the illegitimacy of the previous move.

If the passive player knocks, she immediately becomes the active player and the
previous active player the passive one.

Should the passive player knock even though the active player did nothing wrong,
a single warning is issued against the passive player. Should they knock incorrectly
again, they lose the game.

##End of the Game
The game ends when a player has all board cards on her right side face-up, and
she has no cards in her stacks. That player is the winning player.

##Edgecases
Since turning around stack B and subsequently taking a card from stack A is
considered a single action, merely turning around stack B is knockable. It usually
is anyways because touching stack B is knockable unless the required action is
moving a card from stack B to a final stack.

If the active player has a single card left in their own stacks, and moving it either
to the board in general, or not moving it to a final stack is knockable, and the
passive player knocks, the card is returned to the originating stack.
