'simulation-basic categorization game' provides code to simulate reinforcement with punishment learning in the categorization game. This is the model described in section 3, and for which results are presented in section 4. 

'simulation-categorization game with invention and forgetting' provides code to simulate learning in the categorization game on the modified dynamics featuring invention and forgetting. This is the model discussed in section 5.

'generate figures' provides code that takes the outputs of the main simulation loop and prints six items:

1) the final probability with which an optimal partition is used
2) the players' mean cumulative success rate
3) the players' mean success rate over the last 1000 steps of a run
4) the mean of the maximum final probability associated with a single partition
5) the proportion of runs ending close to a separating equilibrium in the corresponding collapsed game
6) the proportion of runs ending close to a pooling equilibrium in the corresponding collapsed game

The eight .pkl files include all the simulation results reported in the paper. the 'load' function unpickles the data contained in each file, allowing them to be fed (as lists) into the 'show_results' function in 'generate figures'. 

Required packages:

numpy
pickle
matplotlib
joblib
