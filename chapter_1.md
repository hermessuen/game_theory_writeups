## War of Attrition
Two players are involved in a dispute over an object. The value of the object to player i is vi > 0. Time is modeled as a continuous variable that starts at 0 and runs indefinitely.Each player chooses when to concede the object to the other player; if the first player to concede does so at time t, the other player obtains the object at that time. If both players concede simultaneously, the object is split equally between them, player i receiving a payoff of vi/2. Time is valuable: until the first concession each player loses one unit of payoff per unit of time.

NASH EQUILIBRIUM TO THIS GAME

How do we formulate this is a simple strategic game? A strategic game is modeled as the tuple: <N, Ai, xj U>, where N is the number of players, Ai is the set of all possible actions taken by player i and Ui is the total **utility** assigned to player i given a set an **action profile** a: (a1, a2..an) of all of the players within the game . We can also re-formulate U as a **preference relation** for player i, which is essentially a preference over that players individual actions, given a set of actions from all of the other players

A **Nash Equilibrium** is a set of **strategies** for all players (in a simple strategic game, this would be a single decision point) in which no player is incentivised to try to deviate (they can not improve their own payoff or utility by changing strategies. If we want to find the Nash Equilibrium to this game, we need to first find all of the cases in which neither of the two players has an incentive to switch. To simplify the problem, we assume that each player picks one move, _when to concede_. Lets model this is ti and tj, denoting the times that a player concedes. if ti == tj, both players receive pay off vi / 2. This is not a Nash equilibrium solution because either player could switch stratgy to ti + e or tj +e to obtain payoff of vi. Therefore, we must have ti < tj.

If ti < tj, then player j receives payoff (vj - ti), and player i receives pay off "-ti". The key to this problem is to realize that one is **losing value** every second, it is not the final outcome of the game (as intuitively one might think). Therefore, if 0 < ti < tj, player i will move towards 0 to increase expected payoff (less negative). Therefore all Nash Equilibrium to this game have 0=ti < tj. 


## Second Price Auction
Consider now the game where we have a set of N players again. They want to bid on an item. Each player values the item as follows: v1 > v2 > .... vn. The game is modeled as follows, the Action set Ai for each player is the set of R+ and a preference relation over what they would bid for all possible bids of other players. Rather than enumerate all of the possible preference relations, we look at the utility a player could gain by exercising one of the actions in their set, Bi, as vi - bi. In a second price auction, the highest bidder wins, but pays the price of the second highest bid. 

```
Show that in a second price auction the bid vi of any player i is a weakly dominant action: player i’s payoff when he bids vi is at least as high as his payoff when he submits any other bid
```
An **action profile** for this game is the tuple <b1, b2...bn> where bi are the bids of each player. Suppose we have the following Nash Equilibrium: (v1, 0, 0...). As in, player 1 bids how much she values the item, and all of the other players bid 0. Player 1 gets payoff v1 (the amount he values the item), and all other players get payoff 0. No player is incentivised to change strategy, because for every bid bi for player i, bi <= vi < v1. Thus the payoff for all players except player 1 will either be 0 or negative regardless of what they bid, and they will not move. Thus, for player i, who is bidding 0, there is a weakly dominant strategy where bi = e, where 0 + e <=vi, such that the expected payoff for player i is still the same. 

There is also a weird situation in which player 1 may not win the game. In order to see this, consider the profile (v2, v1, 0, 0...). Player 2 wins the auction at price v2 (because it is the _second_ price that they pay. First, let's prove that this is a Nash Equilibrium. We can use the logic from above to show that player i, where i > 2, are in a Nash equilibrium (with their strategies being weakly dominated). Player 1 is in a Nash equilibrium because their payoff is 0, and if they increase their bid to win (they have to be > v1), which moves their payoff to 0. Player 2 also gets payoff 0 for their bid, and cannot improve by changing either. This is _inefficient_ compared to the first case because now we have situation where the total outcome of the game is 0 (no player is given any positive utlity), but we are in an equilibrium (of course we would prefer the first case!)


**Follow up**: the degenerate case happens because of the second price quirk of this auction. Imagine instead that it was the third price. 









