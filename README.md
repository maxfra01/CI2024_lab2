## Strategies

To solve the TSP problem I implemented three strategies: Greedy, Local Search and Evolutionary.
The first one simply chooses the nearest city to the current one. The local search algorithm uses a simulated annealing approach to improve the greedy solution. 
The Evolutionary strategy uses a combination of "inver over" crossover and inversion mutation to evolve the population of solutions.

## Results

| Instance |Greedy strategy (km)| Local search cost (km) | Evolutionary strategy cost (km)|
|:--------:|:------------:|:------------:|:---------------------:| 
| *Vanuatu*   | 1475      | 1345          | 1345                  |
| *Italy* |   4436 | 4182 | **4182** |
| *Russia* | 42334 | 36102 | **35457** |
| *Us* | 48050 | **41462** | 42866 |
| *China* | 63962 |**58040**  | 60992 | 

As we can see in the first three instance, the Evolutionary strategy is the best one. However, in the last two instances the Local Search strategy is the best one. Maybe increasing the number of generations or the population size could improve the results, however, that would lead to a very slow algorithm. 