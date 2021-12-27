# Intelligent-Traffic-Light-via-Reinforcement-Learning
All the videos are played at 15x speed.

Cars with colors of blue, red, green, and yellow are for straight, left-turn, right-turn, and U-turn.

Policy A vs Policy B. (Policy A: variable time interval. Policy B: fixed time interval.)  
Policy A  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/ppo_var_gif.gif) 
Policy B  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/ppo_fix_gif.gif) 

Policy A in the scenario of environment disturbance on an incoming road. (A collision on the incoming east road.)
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/ppo_inc_gif.gif)

Policy A in the scenario of 10% action disturbance. (10% traffic light malfunction.)
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/ppo_act_gif.gif)

Policy A in the scenario of unbalanlced traffic flow rates. (The balanced flow rates are applied within the first 500 seconds. Then, the flow rates in the incoming east road are reduced by three-fourth for another 500 seconds while the flow rates keep the same in other incoming roads. At last, during the third 500 seconds, the flow rates in the incoming east road are back to normal while the other incoming roads’ flow rates are reduced by three-fourth.)
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/ppo_unb_gif1.gif)

Policy A in the scenario of extremely unbalanced traffic flow rates. (Zero flow rates on incoming east and south roads.)
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/ppo_exunb_gif.gif)
