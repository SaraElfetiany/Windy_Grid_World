# Windy_Grid_World

Consider the game depicted in the following diagram:

![image](https://user-images.githubusercontent.com/101424965/200913226-76bee01b-d85b-4de7-a3f0-615a0b3323c6.png)

You are to implement several algorithms to solve this problem:
1. Sarsa
2. Q-learning

Compare all solutions in terms of the optimal policies and episodes necessary for convergence. Select
the best values for 𝜀 and 𝛼 for each case. If they are different, discuss why.

Re-solve the windy gridworld task with King’s moves, assuming that the effect of the wind, if there is
any, is stochastic, sometimes varying by 1 from the mean values given for each column. That is, a third
of the time you move exactly according to these values, as in the previous exercise, but also a third of
the time you move one cell above that, and another third of the time you move one cell below that.

For example, if the agent is one cell to the right of the goal and it chooses to move left, then one-third of
the time the agent will move one cell above the goal, one-third of the time you move two cells above
the goal, and one-third of the time you move to the goal. YOU SHOULD ONLY USE THIS APPROACH.

Mathematically, when the wind is defined by 𝑤, the location of the agent in 𝑦 after the execution of the
action without stochastic wind will be 𝑦 = 𝑎(𝑠) + 𝑤. Then, the stochastic output 𝑦! will be:

<img width="244" alt="image" src="https://user-images.githubusercontent.com/101424965/200913460-6c607a68-d01c-4f66-91bf-5a3b686c88b1.png">
