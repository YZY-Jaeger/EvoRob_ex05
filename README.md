# EvoRobotics Group Assignment

## Team Members
- **Minsol Kim**
- **Yu Zeyuan**

## Project Files and Directory Structure
- `evolution.py`: Contains the primary evolutionary algorithm implementation with elitism strategy.
- `evolution2.py`: Contains additional evolutionary algorithm variants with parameter tweaks.
- `functions.py`: Defines the Ackley function and fitness evaluation function.


- `main.py`: Runs the evolutionary algorithm with initial parameters and plots the results.
- `plot1.png`: Plot of best and average fitness for the initial set of parameters.


- `main2.py`: Runs the evolutionary algorithm with varied parameters for tuning and comparison, and plots the results.
- `plot_psize30.png`: Plot of best and average fitness for population size 30 across different mutation rates.
- `plot_psize100.png`: Plot of best and average fitness for population size 100 across different mutation rates.


## Task Descriptions

### Task 1: Implement a Complete Evolutionary Algorithm
**Files:**
- `main.py`
- `plot1.png`

For this task, we implemented a complete evolutionary algorithm using the following components:

- **Population Size:** Various sizes tested, initially set to 50.
- **Selection Method:** Tournament selection.
- **Replacement Strategy:** Elitism, where a portion of the best individuals are carried over to the next generation.
- **Mutation Rate:** Initial experiments with a mutation rate of 0.1.
- **Recombination:** Simulated binary crossover (SBX) with a probability of 0.9.

### Task 2: Tweak Your Parameters
**Files:**
- `main2.py`
- `plot_psize30.png`
- `plot_psize100.png`

In this task, we explored the effects of different parameters on the evolutionary algorithm's performance. We varied the following parameters:

**Parameters Tested:**
```python
pop_sizes = [30, 100]
mutation_rates = [0.01, 0.05, 0.1]
num_generations = 100  # Fixed
tournament_sizes = [2, 3, 5]
prob_crossover = 0.9  # Fixed
elite_size = 5        # Fixed

Each combination of population size and mutation rate was run, and the best and average fitness values were plotted for comparison. The results were saved as `plot_psize30.png` and `plot_psize100.png`.

