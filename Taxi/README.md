# About

The Taxi Problem from "Hierarchical Reinforcement Learning with the MAXQ Value Function Decomposition" by Tom Dietterich
    
**Description:**  
There are four designated locations in the grid world indicated by R(ed), G(reen), Y(ellow), and B(lue). When the episode starts, the taxi starts off at a random square and the passenger is at a random location. The taxi drives to the passenger's location, picks up the passenger, drives to the passenger's destination (another one of the four specified locations), and then drops off the passenger. Once the passenger is dropped off, the episode ends.
    
**Observations:**   
There are 500 discrete states since there are 25 taxi positions, 5 possible locations of the passenger (including the case when the passenger is in the taxi), and 4 destination locations. 
    
**Passenger locations:**  
- 0: R(ed)
- 1: G(reen)
- 2: Y(ellow)
- 3: B(lue)
- 4: in taxi

**Destinations:**  
- 0: R(ed)
- 1: G(reen)
- 2: Y(ellow)
- 3: B(lue)

**Actions:**  
There are 6 discrete deterministic actions:  
- 0: move south
- 1: move north
- 2: move east 
- 3: move west 
- 4: pickup passenger
- 5: dropoff passenger

**Rewards:**  
There is a default per-step reward of -1, except for delivering the passenger, which is +20, or executing "pickup" and "drop-off" actions illegally, which is -10.

**Rendering:**  
- blue: passenger
- magenta: destination
- yellow: empty taxi
- green: full taxi
- other letters (R, G, Y and B): locations for passengers and destinations

state space is represented by: (taxi_row, taxi_col, passenger_location, destination)

# Version
* [Taxi-v3](https://github.com/openai/gym/blob/8e5a7ca3e6b4c88100a9550910dfb1a6ed8c5277/gym/envs/__init__.py#L183)
>```
id='Taxi-v3',
entry_point='gym.envs.toy_text:TaxiEnv',
reward_threshold=8, # optimum = 8.46
max_episode_steps=200,
```

# Source
* [https://gym.openai.com/envs/Taxi-v3/](https://gym.openai.com/envs/Taxi-v3/)
* [https://github.com/openai/gym/blob/master/gym/envs/toy_text/taxi.py](https://github.com/openai/gym/blob/master/gym/envs/toy_text/taxi.py)
