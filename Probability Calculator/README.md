# Probability Calculator

The main file, `main.py`, serves as an entry point for running and testing the probability calculator program provided by the `prob_calculator` module. This program simulates drawing balls from a hat and calculates the probability of drawing a specified combination of balls. Below, you will find an explanation of how to use the main file and how to run unit tests to ensure that the probability calculator functions correctly.

## Usage

### Importing Modules and Classes

```python
import prob_calculator
from unittest import main
```

The main file begins by importing the necessary modules and classes from the `prob_calculator` module. Specifically, it imports the `Hat` class for creating a hat object with colored balls and the `experiment` function for simulating experiments and calculating probabilities.

### Creating a Hat and Performing Experiments

You can create a hat with a specific configuration of colored balls and perform experiments to calculate probabilities. Here's an example of how to use the program:

```python
hat = prob_calculator.Hat(blue=4, red=2, green=6)
probability = prob_calculator.experiment(
    hat=hat,
    expected_balls={"blue": 2,
                    "red": 1},
    num_balls_drawn=4,
    num_experiments=3000)
print("Probability:", probability)
```

In this example, a hat is created with four blue, two red, and six green balls. The program then performs 3000 experiments where it draws four balls from the hat and calculates the probability of drawing two blue balls and one red ball. The result is printed to the console.

### Running Unit Tests

To verify the correctness of the probability calculator functions, the main file utilizes the `unittest` framework to run unit tests automatically. You can run the tests using the following line of code:

```python
main(module='test_module', exit=False)
```

This line of code automatically discovers and runs the unit tests associated with the `prob_calculator` module.

## Purpose

The main file is designed to showcase how to create a hat with colored balls, simulate experiments, and calculate probabilities based on the specified conditions. It serves as a tool for experimenting with different configurations and testing the accuracy of the probability calculations.

## Development and Testing

During development, the main file allows you to test and verify the functionality of the probability calculator. You can create hats with different configurations, perform experiments, and calculate probabilities for various scenarios. Additionally, running unit tests ensures the accuracy of the probability calculations.

## Usage Example

```python
import prob_calculator
from unittest import main

prob_calculator.random.seed(95)
hat = prob_calculator.Hat(blue=4, red=2, green=6)
probability = prob_calculator.experiment(
    hat=hat,
    expected_balls={"blue": 2,
                    "red": 1},
    num_balls_drawn=4,
    num_experiments=3000)
print("Probability:", probability)

main(module='test_module', exit=False)
```

This code demonstrates how to use the probability calculator program to create hats, simulate experiments, and calculate probabilities. Additionally, it includes unit tests to ensure the accuracy of the probability calculations.
