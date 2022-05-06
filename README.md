# Reinforcement-Learning-with-Space-Invaders.-First-approach

For this project, I just wanted to dive into the Reinforcement Learning world and the best and most entertaining way was through video games. Space Invaders was and still is an iconic Atari game from the '80s and will be the environment where the agent will be trained.

Basicly,  this is the structure of the learning process

<p align='center'>
  <img src='https://user-images.githubusercontent.com/90570944/167203518-c0ff4826-da6b-4cbc-a060-3006c47f05da.png'>
</p>

Its components are:

- Agent: the decision-maker to train.

- Environment: the general setting where the agent learns and decides what actions to take.

- Action 𝑎: one among the set of possible actions the agent can perform

- State 𝑠: condition that the agent is in

- Reward 𝑟: the gain or loss the agent receives from the environment as a result of its own action

- Policy 𝜋: the strategy that the agent chooses to pursue. It represents a mapping between the set of situations and the set of possible actions.

The process follows the following schema: we install the required packages and ROMs, then we create the environment, test the game over 10 episodes. After that we procced to build Neural Network model

<p align='center'>
  <img src='https://user-images.githubusercontent.com/90570944/167206166-dab916a2-1b92-4739-aa5f-80b9d893cd26.png'>
</p>

Subsequently, the agent is built and trained for 10000 steps. Finally, we test the agent's performance via scores.

<p align='center'>
  <img src='https://user-images.githubusercontent.com/90570944/167206754-f7839839-f8c5-439d-8a72-d084f4438f4f.png'>
</p>

The agent's performance was very satisfactory, however, for further trials, some parameters might be tweaked such as the number of steps from 10000 to 1000000, the learning rate from 1e-3 to 1e-4 and so on and so forth. In case you want to kill sometime playing Space Invaders while the model is training, here is a quick way to do it

from gym.utils.play import play

play(gym.make('SpaceInvaders-v0')) #dont forget to run it locally ;)
