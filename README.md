# SnakeGame-AI

This project aims to create an artificial intelligence model for the [Snake](snake-wiki) game. The goal of the snake is to eat the food continuosly. The snake dies on hitting the boundaries or hitting itself. The project is based on Reinforcement Learning.

# Algorithm

We have snake and food on the board randomly placed.
1. We calculate the state of the snake using the 11 values and if any of the conditions is true then set that value to zero else set one. The 11 state values (in order) are as follows:
  * danger straight
  * danger right
  * danger left
  * moving direction left
  * moving direction right
  * moving direction left
  * moving direction up
  * moving direction down
  * food left
  * food right
  * food up
  * food down

2. After getting these states, the agent would pass this to the model and get the next move to perform.
3. After executing the next state calculate the reward. Rewards are defined as below:
  * Eating Food: +10
  * Dying or not eating food for too long: -10
  * Else: 0

4. Updating the Q value using the Bellman Equation.




 

