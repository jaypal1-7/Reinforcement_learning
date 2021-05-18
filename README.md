# Reinforcement_learning
This is an implementatio of a small find the park route game using reinforcement learning.

# overview
A 4x4 maze is used for this perticular game. It follows a reward system for calculation of best path to reach to park. Initially, it uses exploration policy to find better rewards and on findingpositive rewards it tries to exploit it for the maximaiztion of total rewards. It uses transition state matix and action matrix for calculation of Q table. On multiple iterations, the weights of Q table adjusted according to the state matrix and action matrix. On the basis of Q table values, Best path has been choosen for the agent.

# Functioning
1) A 4x4 map was build with a total 16 no. cells.
2) Reward_mateix was designed on the basis of possible routes having different obstacles(dogs= -10) and extra rewards(candies= +50).
3) Transition state matrix is designed on the basis of possible transition from one cell to next cell in any direction. Here, five cases were cosidered for each movement. Up,Down,Left,Right,Neutral(staying in same cell)
4) Action Matrix is designed on the basis of no. of possible action for agent in any cell. Here, the action refers to possible moves in all directions.
5) Q table is calculated with tha help of Bellman's equation. All the values of Q table has been calculated using transistion state matrix and action matrix.
6) Best route is calculated from the values in Q table inorder to maximize the reward.

# Reference
https://www.freecodecamp.org/news/an-introduction-to-q-learning-reinforcement-learning-14ac0b4493cc/
