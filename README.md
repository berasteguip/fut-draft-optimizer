# FIFA Ultimate Team Optimizer ⚽️
This project uses Mixed-Integer Linear Programming (MILP) to solve the problem of selecting an optimal football team (FIFA Ultimate Team–style). The main objective is to maximize the team’s overall rating while respecting constraints on budget, tactical positions, and player chemistry.

## 📋 Project Features
Mathematical Optimization: Formulation based on a model of sets, parameters, and decision variables.

*Realistic Constraints*: Includes budget limits (€500M), minimum average pace, specific attribute requirements for the defensive line, and chemistry requirements.

*4-3-3 Formation*: The model selects exactly 11 players to cover specific positions (GK, LB, CI, CD, RB, MI, CM, MD, LW, ST, RW).

*Visualization*: Automatic generation of a graphical representation of the optimal starting eleven on a football pitch.

## 📁 File Structure
- optimizer.ipynb: Main script. Contains the optimization model developed in Pyomo and the generation of results.

- data_processer.ipynb: Support script used for data cleaning, filtering, and generation of the initial chemistry graph.

- data/: Folder containing player datasets and chemistry links (sample_chemistry_edges_fifa18.csv).

## 🚀 Execution Instructions
To obtain the optimal team, you only need to interact with the optimization file:

*Prerequisites*: Make sure the required libraries are installed:

```bash
pip install pandas pyomo numpy matplotlib
```

### Important note:
There is one cell that takes a few minutes to run, but once executed it does not need to be run again.

## Execution:
Open and run all cells in optimizer.ipynb.

The script will load the preprocessed data from the data/ folder.

At the end, a DataFrame summarizing the team will be printed and the image of the optimal formation will be displayed.

## 🛠️ Technologies Used
*Language*: Python 3.11

*Modeling*: Pyomo (Python Optimization Modeling Objects)

*Solver*: Gurobi / CBC

*Data Analysis*: Pandas / NumPy

*Visualization*: Matplotlib

## Authors
Final project for the course Optimization and Simulation: Pablo Berástegui, José María Benítez, Daniel Escobosa, and Alejandro de Haro.
