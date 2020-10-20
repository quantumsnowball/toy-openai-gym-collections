# Toy OpenAI Gym Collections
The best way to learn programming is to build from scratch on top of a very simple hello world program. The best way to learn reinforcement learning is to start from one of the most simple toy OpenAI Gym which is similar to the real world problem. I organize the directories of this repository by OpenAI Gym environment names. Each environment may represents more than one problem, while each problem may have multiple approaches to solve, therefore each directory may have more than one Jupyter Notebooks files.

# Toy Environment Results
This table shows the results of each approaches that I have tried to solve a particular environment:

| Environment | Q-Learning | DQN |
|:-:|||
| Taxi        | &#9745; | &#9745; |
| CartPole    | &#9744; | &#9744; |
| LunarLander | &#9744; | &#9744; |


# Comparison of Common Reinforcement Learning Algorithms
The following table shows some commonly used reinforcement learning algorithm

| Algorithm 	| Description 	| Model 	| Policy 	| Action Space 	| State Space 	| Operator 	|
|:-:	|:-:	|:-:	|:-:	|:-:	|:-:	|:-:	|
| Monte Carlo 	| Every visit to Monte Carlo 	| Model-Free 	| Either 	| Discrete 	| Discrete 	| Sample-means 	|
| Q-learning 	| State–action–reward–state 	| Model-Free 	| Off-policy 	| Discrete 	| Discrete 	| Q-value 	|
| SARSA 	| State–action–reward–state–action 	| Model-Free 	| On-policy 	| Discrete 	| Discrete 	| Q-value 	|
| Q-learning - Lambda 	| State–action–reward–state with eligibility traces 	| Model-Free 	| Off-policy 	| Discrete 	| Discrete 	| Q-value 	|
| SARSA - Lambda 	| State–action–reward–state–action with eligibility traces 	| Model-Free 	| On-policy 	| Discrete 	| Discrete 	| Q-value 	|
| DQN 	| Deep Q Network 	| Model-Free 	| Off-policy 	| Discrete 	| Continuous 	| Q-value 	|
| DDPG 	| Deep Deterministic Policy Gradient 	| Model-Free 	| Off-policy 	| Continuous 	| Continuous 	| Q-value 	|
| A3C 	| Asynchronous Advantage Actor-Critic Algorithm 	| Model-Free 	| On-policy 	| Continuous 	| Continuous 	| Advantage 	|
| NAF 	| Q-Learning with Normalized Advantage Functions 	| Model-Free 	| Off-policy 	| Continuous 	| Continuous 	| Advantage 	|
| TRPO 	| Trust Region Policy Optimization 	| Model-Free 	| On-policy 	| Continuous 	| Continuous 	| Advantage 	|
| PPO 	| Proximal Policy Optimization 	| Model-Free 	| On-policy 	| Continuous 	| Continuous 	| Advantage 	|
| TD3 	| Twin Delayed Deep Deterministic Policy Gradient 	| Model-Free 	| Off-policy 	| Continuous 	| Continuous 	| Q-value 	|
| SAC 	| Soft Actor-Critic 	| Model-Free 	| Off-policy 	| Continuous 	| Continuous 	| Advantage 	|
Source: [Wikipedia](https://en.wikipedia.org/wiki/Reinforcement_learning#Comparison_of_reinforcement_learning_algorithms)