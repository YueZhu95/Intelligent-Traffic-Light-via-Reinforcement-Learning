# Intelligent-Traffic-Light-via-Reinforcement-Learning
Thesis videos are for the paper: Intelligent Traffic Light via Policy-based Deep Reinforcement Learning. The URL for the paper is shown below:  
http://arxiv.org/abs/2112.13817

All the videos are played at 15x speed.

Cars with colors of purple, red, green, and yellow are for straight, left-turn, right-turn, and U-turn.

Predefined: repeatedly loop the traffic light phase from the first phase to the last one.  

Policy A: intelligent traffic light with PPO for the traffic light phases with variable time intervals trained in the scenario of balanced traffic.  

Policy B: intelligent traffic light with PPO for the traffic light phases with fixed time intervals trained in the scenario of balanced traffic.  

Policy D: trained in the scenario of complex traffic flows consisting of balanced and unbalanced traffic based on intelligent traffic light with PPO for the traffic light phases with variable time intervals.(The balanced flow rates are applied within the first 500 seconds. Then, the flow rates in the incoming east road are reduced by three-fourth for another 500 seconds while the flow rates keep the same in other incoming roads. At last, during the third 500 seconds, the flow rates in the incoming east road are back to normal while the other incoming roads’ flow rates are reduced by three-fourth.)

### Intelligent traffic lights trained via different DRL methods
Predefined (Vehicle passing time (s): 1800, Vehicle waiting time (s): 132713)  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/predefined_gif.gif) 

DQN (Vehicle passing time (s): 1252, Vehicle waiting time (s): 77570)  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/dqn_gif2.gif) 

Policy B (Vehicle passing time (s): 1181, Vehicle waiting time (s): 59677)  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/ppo_fix_gif2.gif) 

### Traffic light phases with variable intervals
Policy A (Vehicle passing time (s): 1076, Vehicle waiting time (s): 55028)  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/ppo_vari_gif.gif) 

### Environment disturbances

The environment disturbance is due to the occurrence of traffic collisions. There is a 2% probability with which a driver may not follow the traffic laws and cause the crash. A traffic collision stays for 300 seconds, then the vehicles involved in the crash are removed and have no further impact on the traffic flow. Here shows the videos of the traffic collisions on an incoming road.

Predefined (Vehicle passing time (s): 1820, Vehicle waiting time (s): 135117)  
The fourteenth car on the inside lane of the incoming east road has the accident.  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/Predefined_inc_gif.gif) 

Policy A (Vehicle passing time (s): 1271, Vehicle waiting time (s): 69884)  
The fourth car on the outside lane of the incoming east road has the accident.  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/PA_inc_gif.gif) 

### Action disturbances (10%)

Action disturbances can happen due to the malfunction of the traffic light. After a light phase is determined, the traffic light has a probability of 90 percent to switch to the desired light phase and a probability of 10 percent to switch to one of the other phases randomly.

Predefined (Vehicle passing time (s): 1942, Vehicle waiting time (s): 139863)  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/Predefined_act_gif.gif) 

Policy A (Vehicle passing time (s): 1187, Vehicle waiting time (s): 58389)  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/PA_act_gif.gif) 

### Unbalanced traffic flows

The balanced flow rates are applied within the first 500 seconds. Then, the flow rates in the incoming east road are reduced by three-fourth for another 500 seconds while the flow rates keep the same in other incoming roads. At last, during the third 500 seconds, the flow rates in the incoming east road are back to normal while the other incoming roads’ flow rates are reduced by three-fourth.

Policy A for complex traffic flows (Vehicle passing time (s): 3041, Vehicle waiting time (s): 233483)  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/PA_unb_gif.gif) 

The extremely unbalanced traffic flows have zero incoming traffic flow rates on the incoming east and south roads.

Policy A for extremely unbalanced traffic flow (Vehicle passing time (s): 1000, Vehicle waiting time (s): 23679)  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/PA_exunb_gif.gif) 

Policy D for extremely unbalanced traffic flow (Vehicle passing time (s): 865, Vehicle waiting time (s): 18372)  
![image](https://github.com/YueZhu95/Intelligent-Traffic-Light-via-Reinforcement-Learning/blob/main/PD_exunb_gif.gif) 
