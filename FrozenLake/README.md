# About

Winter is here. You and your friends were tossing around a frisbee at the park when you made a wild throw that left the frisbee out in the middle of the lake. The water is mostly frozen, but there are a few holes where the ice has melted. If you step into one of those holes, you'll fall into the freezing water. At this time, there's an international frisbee shortage, so it's absolutely imperative that you navigate across the lake and retrieve the disc. However, the ice is slippery, so you won't always move in the direction you intend.

The surface is described using a grid like the following:  

```
SFFF
FHFH
FFFH
HFFG
```   
```
S : starting point, safe  
F : frozen surface, safe  
H : hole, fall to your doom  
G : goal, where the frisbee is located  
```

The episode ends when you reach the goal or fall in a hole.

You receive a reward of 1 if you reach the goal, and zero otherwise.

# Version
* [FrozenLake-v0](https://github.com/openai/gym/blob/8e5a7ca3e6b4c88100a9550910dfb1a6ed8c5277/gym/envs/__init__.py#L150)
    ```
    id='FrozenLake-v0',
    entry_point='gym.envs.toy_text:FrozenLakeEnv',
    kwargs={'map_name' : '4x4'},
    max_episode_steps=100,
    reward_threshold=0.78, # optimum = .8196
    ```
* [FrozenLake8x8-v0](https://github.com/openai/gym/blob/8e5a7ca3e6b4c88100a9550910dfb1a6ed8c5277/gym/envs/__init__.py#L158)
    ```
    id='FrozenLake8x8-v0',
    entry_point='gym.envs.toy_text:FrozenLakeEnv',
    kwargs={'map_name' : '8x8'},
    max_episode_steps=200,
    reward_threshold=0.99, # optimum = 1
    ```

# Source
* <https://gym.openai.com/envs/FrozenLake-v0/>
* <https://gym.openai.com/envs/FrozenLake8x8-v0/>
* <https://github.com/openai/gym/blob/master/gym/envs/toy_text/frozen_lake.py>