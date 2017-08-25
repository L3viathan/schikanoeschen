# League Rules

These league rules apply to the league of a certain `#schika` channel on a
certain Slack team that shall remain unnamed.

## Membership and Ranked Games

Through playing a ranked game against an active member of the league, one
becomes a member of the league. New members start with rank 1000. When a player
becomes inactive (by not having played a league game in two months, or by
explicit wish), they are marked as such and no longer shown in the official
rank table, though their rank remains stored. When they express they want to
become an active player again, or through playing a ranked game against another
active member, they become active again.

A game between two active players is a ranked game, unless both players agree
before the game that it shall be unranked.

All ranked games are played according to the official game rules. If both
players agree before the game, they may also play a ranked game with modified
rules, but this has to be stated before each such game.

## Ranking and the ELO system

The ranking is based on the [ELO ranking
system](https://en.wikipedia.org/wiki/Elo_rating_system).

After a player has played a game, their new score is computed by the formula
below.

    k = 16
    S = 1 if you win, 0 if you lose, 0.5 if you draw
    r(someone) = old rank of someone
    R(someone) = 10**(r(someone)/400)
    new rank := round(r(you) + k*(S-R(you)/(R(you)+R(other))))

@l3viathan is responsible for the technical implementation of both storage and
calculation of ranks.

## Changes to game rules

Changes can be made to the game rules by the following voting system. It is not
anonymous.

1. Fork this repository, make the proposed change in the game rules (preferably
   in both languages).
2. Make a pull request to this repository.
3. Announce the request in `#schika`, even if it was automatically posted
   there, along with a time limit, which may not be less than one week from the
   moment the announcement is made.
4. If, before the time limit is up, every active player agrees to the rules (by
   emoji reaction), the proposal is accepted.
5. If the time limit is up and not every active player has agreed to the rules,
   every player who hasn't voted is assumed to having voted in favor. After
   this adjustment, the proposal is accepted if more players voted in favor
   than against it. In case of a draw, the proposal is rejected.
6. If the proposal is rejected, the pull request is closed.
7. If the proposal is accepted, the pull request is merged and the new rules
   are in effect.

## Changes to league rules

Changes can be made to these league rules by the following voting system. It is
not anonymous.

1. Fork this repository, make the proposed change in the league rules
   (preferably in both languages).
2. Make a pull request to this repository.
3. Announce the request in `#schika`, even if it was automatically posted
   there, along with a time limit, which may not be less than one week from the
   moment the announcement is made.
4. If, before the time limit is up, every active player agrees to the rules (by
   emoji reaction), the proposal is accepted
5. If the time limit is up and not every active player has agreed to the rules,
   every player who hasn't voted is assumed to having voted in favor. After
   this adjustment, the proposal is accepted if more players voted in favor
   than against it. In case of a draw, the proposal is rejected.
6. If the proposal is rejected, the pull request is closed.
7. If the proposal is accepted, the pull request is merged and the new rules
   are in effect.
