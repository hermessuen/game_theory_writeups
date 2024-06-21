Recall what a simple strategic game is:
1. You have a set number of players N, which with a set of Actions available to them
2. All players make a decision, resulting in an Action Profile for the game
3. This Action profile of the game results in a payoff for each player, the exact value of which is determined by each player's utility function (see below)

Neumann's Utility Theory:
- Assuming a risky set of options open to an individual, and we set some set of initial and easy axioms as to how they would act, then an individual will simply act AS IF they are maximizing a scalar utility.
- Put another way, when we are rational, our actions can be explained by maximizing the scalar value coming from a straightforward utility function. 


### Beauty Game Contest
Pick a number between 1 & 100. If I ask a room of 100 people to do this, the winner who picks the number closest to 2/3 of the average number that everyone picked will win. What is the right number to pick?
An intuitive strategy is to first think what the average number everyone would pick and then pick 2/3 of that. If it were just you playing this game, it would be easy, you would think to yourself:
"what is the most likely number everyone would pick (or put a probability distribution), and then multiply by 2/3 and pick the group with highest E.V (if we quantize to integers
then it becomes a non-invertible function). 

The reason this is a classic problem in game theory is because all of the other people are aware of the same rule, and therefore,
will also be picking their numbers knowing this fact. How can we know what number to pick, knowing that they are also playing the game?

In the language of game theory, my choice of number is a specific strategy. 

I actually have no idea what to pick. Therefore, I start by ruling out all of the numbers that I know definitely won't work. For example, the max number I could ever pick is 67, since the max possible average would be 100.
Any number above 67 is what is known as a dominated strategy, as in there is another strategy out there that provides for more utility in every possible way.

What is the next step? Think about what happens with other players. "What will they also do?". Assuming they're not idiots, they would probably also recognize this fact and limit their guesses between 1-67.
If that were the case, then in reality, the max value in this new set is (2/3) * 67 = 45. We all know that everyone is guessing between 1-67, and therefore the max value of 2/3 of our average is 45. It is 
now easy to continue this process until we arrive and the optimal answer: **1**. Everyone should pick 1, and everyone will win.

Of course, this doesn't actually happen in practice. People don't think through in the same way that game theorists do. Thus, when playing this game in the real-world, what should one do? 


### Price-Matching 
It's possible to also then frame competitions between companies as a game. Imagine two companies can produce the same goods for cost **X** and they can choose to sell those goods at costs **Y** and **Z** respectively.
Since it is the same goods, consumers are at most willing to pay min(Y, Z). We can now ask the following question: what is the optimal price that both players would set this particular good at? As long as the company
sells their good at a price greater than **X** then they would have made a profit. Thus, in a true bidding war, both companies would sell at a price that is just barely greater than **X**. This is the 
Nash Equilibrium. As long as a company can set their price Y s.t:  **X** < **Y** < **Z**, where **Z** is the price of the competitor, then they will steal all of their competitors customers. If the price is the same, 
customers are split, and each company is incentivized to lower their price slightly s.t to get more share of the customers. 

What if a company offers price-matching? i.e, if a competitor offers a lower price, then we will match. Does the Nash Equilibrium change? Let's reason through this. Essentially: could any player unilaterally improve their
utility by changing strategies? The first case is both companies set the same price above **X** where they make a reasonable profit. In the example above, with no price-matching, this quickly descends the price back down to 
**X**. With Price matching, this means that if I chose to lower my cost, the other competitor would simply match that price, meaning I would not gain any more customers (our customers are still split).
Therefore, whatever profit margin we initially set, I would _lose_ money if chose to set the price lower. Thus, we stay at a Nash Equilibrium! Price-Matching satisfies the companies more than
the consumers...






