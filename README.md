# Monty Hall Analysis

## Overview

This is a learning project designed to explore the Monty Hall problem through data analysis using Python. The Monty Hall problem is a famous probability puzzle that illustrates counterintuitive statistical principles.

### The Monty Hall Problem

In the classic game show scenario:
- There are three doors: behind one is a car, behind the other two are goats.
- The contestant picks one door.
- The host, who knows what's behind each door, opens another door revealing a goat.
- The contestant is then given the choice to switch to the remaining door or stick with their original choice.

The surprising result is that switching doors gives a 2/3 chance of winning the car, while staying only gives 1/3 chance.

This project analyzes simulation data to empirically verify these probabilities.

## Project Structure

- `monty_hall_analysis.ipynb`: The main Jupyter notebook for analysis
- `pyproject.toml`: Project configuration for uv
- `data/monty_hall_sample.csv`: Sample simulation data
- `README.md`: This file

## Data Description

The sample data in `data/monty_hall_sample.csv` contains simulated Monty Hall game trials with the following columns:

- `trial`: Trial number
- `car_door`: Door number (1-3) where the car is located
- `initial_pick`: Contestant's first door choice
- `revealed_door`: Door opened by host (always a goat)
- `final_pick`: Contestant's final choice (after switch/stay decision)
- `strategy`: "Switch" or "Stay"
- `won`: 1 if won car, 0 if not
- `result`: "Win" or "Lose"

## Setup with uv

### Prerequisites

- Python 3.11 or higher
- uv package manager

### Installation Steps

1. **Install uv** (if not already installed):

   ```bash
   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```

   This installs uv, a fast Python package installer and resolver.

2. **Navigate to the project directory**:

   ```bash
   cd /path/to/monty-hall-analysis
   ```

3. **Sync the project environment**:

   ```bash
   uv sync
   ```

   This creates a virtual environment and installs any dependencies specified in `pyproject.toml`.

4. **Open and run the notebook**:

   Open `analysis.ipynb` in VS Code or Jupyter and execute the cells to perform the analysis.

## Learning Objectives

This project helps you learn:

- Understanding probability paradoxes like the Monty Hall problem
- Reading and analyzing CSV data with Python
- Calculating empirical probabilities from simulation data
- Basic data manipulation and statistics
- Using modern Python project management tools (uv)

## Extending the Project

To deepen your learning, consider:

- Analyzing the full dataset to compute win rates for switch vs. stay strategies
- Creating visualizations of the results
- Running your own simulations with more trials
- Exploring variations of the problem (e.g., 4 doors, multiple reveals)

## Resources

- [Monty Hall Problem on Wikipedia](https://en.wikipedia.org/wiki/Monty_Hall_problem)
- [UV Documentation](https://docs.astral.sh/uv/)