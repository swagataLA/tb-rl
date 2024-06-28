# Reinforcement Learning Agent in a Text- based Maze game:
### Description
We implemented a reinforcement learning agent that looks at the sentences received by bots on a maze game and chooses a paths to the goal accordingly.  It uses Q-Learning and SARSA algorithms and we can observe how the agent chooses different paths according to the algorithms they use.

**SARSA(State, Action, Reward, State, Action)**: On-policy value-based approach ->  updated based on the current choices of the policy.

**Q-learning**: An off-policy approach. Differs from SARSA in its update rule by assuming the use of the optimal policy -> takes the action that maximizes the Q value of the next state.

### Environment 
For our environment, we referred to the OpenAI gym library initially to figure out what sort of features were important for an environment to have for an RL agent. Features like getting the valid actions, resetting the maze, update maze after action to name a few.

For our environment we had mazes represented in arrays such as the one shown and had different letters represent different things.  Agent is represented with A, bots are represented with B, goal with a ‘G’ and then we have the pits ‘P’. Goal and the pits are both terminal states. We also introduced another character ‘W’ that represent an obstacle like a wall but that was used for a more complicated maze that we will see later.

Our environment also contains a dictionary for texts associated with the positions of the bots. This method was used for the simplicity of environment.

The project also have two different mazes used but this can be changed in the notebook. Where you can add or remove as many positive or negative bots.

### UI implemented
This also brings a UI where you can see the steps and paths taken by the agent when it finishes learning the best path.

![image](https://github.com/swagataLA/tb-rl/assets/123109547/14d04846-9ef0-4035-b624-73c05eda7e44)
![image](https://github.com/swagataLA/tb-rl/assets/123109547/b5aa8dec-c2f9-491b-be22-36e5d70196d7)


### Future implementation ideas
- Moving bots that follow a specific path
- Make it a multi-agent environment where the bots are also agents
- Make the bot responses more like a story to follow





