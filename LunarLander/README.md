# About
Rocket trajectory optimization is a classic topic in Optimal Control.

According to Pontryagin's maximum principle it's optimal to fire engine full throttle or turn it off. That's the reason this environment is OK to have discreet actions (engine on or off).

* The landing pad is always at coordinates (0,0). 
* The coordinates are the first two numbers in the state vector. 
* Reward for moving from the top of the screen to the landing pad and zero speed is about 100..140 points. 
* If the lander moves away from the landing pad it loses reward. 
* The episode finishes if the lander crashes or comes to rest, receiving an additional -100 or +100 points. 
* Each leg with ground contact is +10 points. 
* Firing the main engine is -0.3 points each frame. 
* Firing the side engine is -0.03 points each frame. 
* Solved is 200 points.

Landing outside the landing pad is possible. Fuel is infinite, so an agent can learn to fly and then land on its first attempt. Please see the source code for details.

To see a heuristic landing, run: 
>`python gym/envs/box2d/lunar_lander.py`

To play yourself, run: 
>`python examples/agents/keyboard_agent.py LunarLander-v2`

Created by Oleg Klimov. Licensed on the same terms as the rest of OpenAI Gym.

# Version
* [LunarLander-v2](https://github.com/openai/gym/blob/8e5a7ca3e6b4c88100a9550910dfb1a6ed8c5277/gym/envs/__init__.py#L97)
    ```
    id='LunarLander-v2',
    entry_point='gym.envs.box2d:LunarLander',
    max_episode_steps=1000,
    reward_threshold=200,
    ```

# Source
* [https://gym.openai.com/envs/LunarLander-v2/](https://gym.openai.com/envs/LunarLander-v2/)
* [https://github.com/openai/gym/blob/master/gym/envs/box2d/lunar_lander.py](https://github.com/openai/gym/blob/master/gym/envs/box2d/lunar_lander.py)