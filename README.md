'simulation-basic categorization game' provides code to simulate reinforcement with punishment learning in the categorization game. This is the model described in section 3, and for which results are presented in section 4. 

'simulation-categorization game with invention and forgetting' provides code to simulate learning in the categorization game on the modified dynamics featuring invention and forgetting. This is the model discussed in section 5.

'generate figures' provides code that takes the outputs of the main simulation loop and prints six items:

1) the final probability with which an optimal partition is used
2) the players' mean cumulative success rate
3) the players' mean success rate over the last 1000 steps of a run
4) the mean of the maximum final probability associated with a single partition
5) the proportion of runs ending close to a separating equilibrium in the corresponding collapsed game
6) the proportion of runs ending close to a pooling equilibrium in the corresponding collapsed game

To generate results, run the desired simulation notebook. The 'save' function allows the output of the main simulation loop to be saved as a pkl file. The 'load' function unpickles the saved data, allowing them to be fed (as a nested list) into the 'show_results' function in 'generate figures'. Alternatively, the 'show_results' function can be copy-and-pasted directly into a simulation notebook and applied to the output.

Required packages:

numpy
pickle
matplotlib
joblib
