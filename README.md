# SmartSnake

Reinforcement Learning(RL) is one of the main types of machine learning algorithms. An agent learns by interacting with its environment: it chooses an action and receives a feedback from the environment ( observations and rewards ), its goal is to maximize the sum of the rewards.

Deep RL is combining deep learning and RL to map inputs to outputs by using the states as the input and values for actions as the output. Rewards are for adjusting the weights.

Finally, the agent learns to predict the best action for a given state.


## Project Development

* snake_game.py : Creating the snake game from scratch using Pygame 
* q_model.py : building the model to predict the next best action using PyTorch
* agent.py : Creating the agent and starting the training
* plotting.py : Creating a function to plot the learning curve during the training

## training...

First steps: 
![Learning 0](https://user-images.githubusercontent.com/88405252/139755077-f4a7d3e9-3b41-4f98-b4b2-b7e83cc2f9fa.gif)

After playing 100 games, the agent reached a score of 48:
![Learning 1](https://user-images.githubusercontent.com/88405252/139755119-f06a9562-17c1-4025-b559-29b56145ef28.gif)

The record is 63 after 230 games:

![Figure_1](https://user-images.githubusercontent.com/88405252/139759930-d2a87792-a9e1-45c9-aa54-6b269d2f10d5.png)


## Notes

* The agent learns to avoid obstacles surrounding the snake’s head, but it can’t see the whole game. So the agent will enclose itself and die, especially when the snake is longer.
* More details in this article
https://towardsdatascience.com/snake-played-by-a-deep-reinforcement-learning-agent-53f2c4331d36
