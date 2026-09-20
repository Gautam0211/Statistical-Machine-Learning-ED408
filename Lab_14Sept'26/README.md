# Genetic Algorithm and Simulated Annealing

## 📌 Project Overview

This project implements two optimization techniques in Python:

1. **Genetic Algorithm (GA)** – A population-based optimization technique inspired by natural selection and evolution.
2. **Simulated Annealing (SA)** – A probabilistic optimization technique inspired by the cooling process of metals.

Both algorithms are implemented separately to understand how optimization works using different strategies.

---

## 🛠️ Technologies Used

* Python 3
* `random` – For random population generation, selection, and mutation.
* `math` – For calculating the acceptance probability in Simulated Annealing.

No external libraries are required.

---

# 1. Genetic Algorithm

## 🎯 Objective

The Genetic Algorithm maximizes the following objective function:

$$
f(n) = n^2 + 3n
$$

The value of `n` is represented using a 6-bit binary chromosome.

### Search Space

$$
0 \leq n \leq 63
$$

The algorithm searches for the chromosome that produces the maximum fitness value.

## ⚙️ Parameters

| Parameter             | Value                    |
| --------------------- | ------------------------ |
| Population size       | 8                        |
| Chromosome length     | 6 bits                   |
| Number of generations | 5                        |
| Crossover type        | Single-point crossover   |
| Crossover point       | 3                        |
| Mutation type         | Bit-flip mutation        |
| Mutation rate         | 0.10                     |
| Elitism               | 1 chromosome             |
| Selection method      | Roulette-wheel selection |

## 🔄 Working Procedure

1. Generate an initial population of 8 random binary chromosomes.
2. Decode each chromosome into a decimal value.
3. Calculate the fitness of every chromosome.
4. Select parents using roulette-wheel selection.
5. Apply single-point crossover at position 3.
6. Apply bit-flip mutation with a probability of 0.10.
7. Preserve the best chromosome using elitism.
8. Repeat the process for 5 generations.
9. Return the chromosome with the highest fitness.

## 📤 Output

The program displays:

* Initial population.
* Best chromosome in each generation.
* Decimal value of the best chromosome.
* Fitness of the best chromosome.
* Final best solution.

---

# 2. Simulated Annealing

## 🎯 Objective

The Simulated Annealing algorithm minimizes the following function:

$$
f(x) = x^2 - 8x + 20
$$

The algorithm begins with an initial solution and explores neighboring solutions while gradually reducing the temperature.

## ⚙️ Parameters

| Parameter           | Value        |
| ------------------- | ------------ |
| Initial solution    | 2            |
| Initial temperature | 20           |
| Cooling factor      | 0.7          |
| Minimum temperature | 0.5          |
| Maximum iterations  | 6            |
| Step size           | 2            |
| Optimization goal   | Minimization |

## 🔄 Working Procedure

1. Start with `x = 2`.

2. Calculate the objective function value.

3. Generate a neighboring solution using:

   `candidate = current_solution + 2`

4. Calculate the change in objective value:

   $$
   \Delta f = f(x') - f(x)
   $$

5. Accept the candidate if it improves the solution.

6. If the candidate is worse, accept it probabilistically using:

   $$
   P = e^{-\Delta f/T}
   $$

7. Reduce the temperature using:

   $$
   T_{\text{new}} = 0.7T
   $$

8. Repeat until 6 iterations are completed or the temperature falls below 0.5.

9. Return the final solution.

## 📤 Output

The program displays:

* Current iteration.
* Current solution.
* Objective function value.
* Temperature.
* Whether the candidate solution was accepted.
* Final solution and minimum function value.

---

## 📁 Project Structure

```text
Genetic-Simulated-Annealing/
│
├── genetic_algorithm.py
├── simulated_annealing.py
└── README.md
```

### File Descriptions

| File                     | Description                       |
| ------------------------ | --------------------------------- |
| `genetic_algorithm.py`   | Implements the Genetic Algorithm. |
| `simulated_annealing.py` | Implements Simulated Annealing.   |
| `README.md`              | Project documentation.            |

---

## ▶️ How to Run

### 1. Clone or download the project

Download the project files to your computer.

### 2. Open a terminal in the project folder

### 3. Run the Genetic Algorithm

```bash
python genetic_algorithm.py
```

### 4. Run Simulated Annealing

```bash
python simulated_annealing.py
```

---

## 📚 Concepts Demonstrated

* Optimization algorithms
* Fitness functions
* Binary chromosome encoding
* Roulette-wheel selection
* Crossover and mutation
* Elitism
* Local search
* Temperature-based exploration
* Cooling schedules
* Probabilistic acceptance of worse solutions

---

## ⚠️ Important Notes

* The Genetic Algorithm performs **maximization**.
* Simulated Annealing performs **minimization**.
* The Genetic Algorithm uses a fixed crossover point of 3.
* The Simulated Annealing neighbor is generated by adding 2 to the current solution.
* Random seeds may be used to make results reproducible.
* The parameters can be changed to study their effect on optimization performance.

---

## 👨‍💻 Author

**Gautam Chhabra**

A Python project demonstrating Genetic Algorithm and Simulated Annealing optimization techniques.
