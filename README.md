# Data-Driven Marketing Attribution

## Game theory and the Shapley value
The Shapley value is a concept taken from cooperative game theory. In a game of multiple players that can work together (form coalitions) to increase the likelihood of a desired outcome (payoff), the Shapley value provides a way to fairly divide the payoff between the players.

Essentially, the Shapley value is a measure of a player's average marginal contribution to each coalition. Taking into consideration that players can join coalitions at different points in time (order), and have varying degrees of influence (worth). Its based on the assumption that each ordering has the same probability of occurring, thus players are awarded by their contribution to all permutations.

In the context of marketing analytics, campaign channels are the players of the game, and the various ways in which the channels interact with accounts throughout the buyer journey form the coalitions. Cooperative game theory and the Shapley value provide a stable way to measure channel influence and fairly divide the credit for sales conversions between the channels, based on their individual contribution to the total payoff.

Marketing benefits:
* Deeper insight into channel performance
* Fair division of credit, based on measured contribution
* Ability to optimise channel spend and influence sales results
* Shapley value is a widely used, and Nobel prize winning, solution

## The characteristic function

A game is defined by a set of players ***N*** and a characteristic function ***v***. Every subset of players is called a coalition ***S***, and the characteristic function ***v(S)*** assigns a value to each coalition to signify it's **worth**. A coalition's worth represents the payoff that it can generate when it's players work together.

Options for defining the characteristic function for marketing include:
* Total revenue generated by each coalition
* Total number of sales conversions generated by each coalition
* Conversion ratio of each coalition (conversions / opportunities)
* Conditional probability of conversion - i.e. likelihood of converting given a set of channels (Naive Bayes)

This [notebook](game_theory_attribution.ipynb) provides an example of how to calculate the Shapley values for three marketing channels with a characteristic function based on conversion ratio.
