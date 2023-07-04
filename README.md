# Reinforcement-Learning-for-Snake
Reinforcement Learning course, CentraleSupélec, Summer 2023

### Goal
Creation of an environment and implementation of several agents to play the Snake game

### Language
```Python```

### Contents
1. Creation of two environments: with and without crossing conditions
2. Creation of the agents: Q-learning, Expected Sarsa, Deep-Q Network
3. Discussions and conclusion

### Results visualization
1. Without crossing conditions
![](https://github.com/AntoineDargier/Reinforcement-Learning-for-Snake/blob/main/snake_game_DQN.gif)

2. With crossing conditions
![](https://github.com/AntoineDargier/Reinforcement-Learning-for-Snake/blob/main/snake_game_ES_bound.gif)

### Libraries
* ```gymnasium```
* ```Pytorch```
* ```imageio```
* ```numpy```
* ```cv2```
* ```matplotlib```

### Conclusion
I could see in this project a large part of the challenges of reinforcement
learning. Indeed, by implementing my environments, I saw that it was
very important to model them well to have efficient agents. The order of the steps,
the rewards, and the stopping conditions are all very important parameters that
must be well understood. I have seen that the Q-Learning agent is very good
to start with: it learns very quickly, but can sometimes fall into circuits where
the snake goes around in circles. Despite my best efforts to help the snake always
head towards the apple, it sometimes gets into loops. The Deep Q-Network model
seems to perform better in all environments, but unfortunately, it takes much
longer to train.

For an even more complete project, I could think about new state models to
avoid crossings, for example by keeping in memory the previous movements.
However, with these first models, I obtained very good results and very satisfactory agents.
