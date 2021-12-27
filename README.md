# Intelligent-Traffic-Light-via-Reinforcement-Learning
All the videos are played at 15x speed.

Cars with colors of blue, red, green, and yellow are for straight, left-turn, right-turn, and U-turn.

Predefined: repeatedly loop the traffic light phase from the first phase to the last one.  

Policy A: intelligent traffic light with PPO for the traffic light phases with fixed time intervals.  

Policy B: intelligent traffic light with PPO for the traffic light phases with variable time intervals.  

Policy D: trained in the scenario of unbalanlced traffic flow rates based on intelligent traffic light with PPO for the traffic light phases with fixed time intervals.

The balanced flow rates are applied within the first 500 seconds. Then, the flow rates in the incoming east road are reduced by three-fourth for another 500 seconds while the flow rates keep the same in other incoming roads. At last, during the third 500 seconds, the flow rates in the incoming east road are back to normal while the other incoming roads’ flow rates are reduced by three-fourth.

### Intelligent traffic lights trained via different DRL methods: DQN and Policy B, and Predefined traffic light
Predefined  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/predefined_gif.gif) 

DQN  


Policy B  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/ppo_fix_gif2.gif) 
