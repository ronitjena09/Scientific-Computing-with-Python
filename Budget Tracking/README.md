# Budget Tracking

The main file, `main.py`, serves as an entry point for the budget tracking program provided by the `budget` module. This program allows you to create and manage categories for tracking expenses, perform various financial operations (deposits, withdrawals, transfers), and generate a spending chart based on the expenses across categories. Below, you will find an explanation of how to use the main file and how to run unit tests to ensure that the budget tracking functions work correctly.

## Usage

### Importing Modules and Classes

```python
import budget
from budget import create_spend_chart
from unittest import main
```

The main file begins by importing the necessary modules and classes from the `budget` module. It specifically imports the `create_spend_chart` function for generating a spending chart and the `Category` class for managing expense categories.

### Managing Expense Categories

The main file demonstrates the creation and management of expense categories. Here's an example of how to work with expense categories:

```python
food = budget.Category("Food")
food.deposit(1000, "initial deposit")
food.withdraw(10.15, "groceries")
food.withdraw(15.89, "restaurant and more food for dessert")
```

In this example, a category named "Food" is created, an initial deposit is made, and two withdrawals are recorded with descriptions.

### Transferring Funds

You can also transfer funds from one category to another:

```python
clothing = budget.Category("Clothing")
food.transfer(50, clothing)
```

In this example, $50 is transferred from the "Food" category to the "Clothing" category.

### Printing Category Information

You can print information about each category, including its ledger and total balance:

```python
print(food)
print(clothing)
```

This code will display the ledger and balance of both the "Food" and "Clothing" categories.

### Generating a Spending Chart

The `create_spend_chart` function is used to generate a spending chart that visually represents the percentage of expenses in each category:

```python
print(create_spend_chart([food, clothing, auto]))
```

This code generates and prints a spending chart based on the expenses recorded in the provided categories.

### Running Unit Tests

To verify the correctness of the budget tracking functions, the main file utilizes the `unittest` framework to run unit tests automatically. You can run the tests using the following line of code:

```python
main(module='test_module', exit=False)
```

This line of code automatically discovers and runs the unit tests associated with the `budget` module.

## Purpose

The main file is designed to showcase how to use the budget tracking program to manage expense categories and generate spending charts. It serves as a useful tool for tracking and visualizing expenses across different categories.

## Development and Testing

During development, the main file allows you to test and verify the functionality of the budget tracking functions. You can create and manage expense categories, perform financial operations, and generate spending charts to ensure that the program meets your financial tracking needs.

## Usage Example

```python
import budget
from budget import create_spend_chart
from unittest import main

food = budget.Category("Food")
food.deposit(1000, "initial deposit")
food.withdraw(10.15, "groceries")
food.withdraw(15.89, "restaurant and more food for dessert")

clothing = budget.Category("Clothing")
food.transfer(50, clothing)
clothing.withdraw(25.55)
clothing.withdraw(100)

auto = budget.Category("Auto")
auto.deposit(1000, "initial deposit")
auto.withdraw(15)

print(food)
print(clothing)

print(create_spend_chart([food, clothing, auto]))

main(module='test_module', exit=False)
```

This code is used for creating, managing, and visualizing expense categories. Additionally, it includes unit tests to ensure the functionality of the budget tracking program.
