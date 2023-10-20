This code is a useful tool for formatting and displaying arithmetic problems for educational purposes and can be easily customized for various use cases.

# # Arithmetic Arranger

The main file, `main.py`, serves as an entry point for running and testing the `arithmetic_arranger` function provided by the `arithmetic_arranger` module. This file is primarily used during development to test the functionality of the arithmetic arrangement program. Below, you will find an explanation of how to use the main file and how to run unit tests to ensure that the `arithmetic_arranger` function functions correctly.

## Usage

### Importing the `arithmetic_arranger` Function

```python
from arithmetic_arranger import arithmetic_arranger
```

The main file begins by importing the `arithmetic_arranger` function from the `arithmetic_arranger` module. This function is responsible for arranging arithmetic problems and, optionally, displaying their solutions.

### Example Usage

In the main file, you can see an example of how to use the `arithmetic_arranger` function:

```python
print(arithmetic_arranger(["32 + 698", "3801 - 2", "45 + 43", "123 + 49"]))
```

Here, a list of arithmetic problems is passed to the `arithmetic_arranger` function. This code snippet demonstrates how to call the function and print the resulting formatted arithmetic problems without showing the solutions.

### Running Unit Tests

To verify the correctness of the `arithmetic_arranger` function, the main file utilizes the `unittest` framework to run unit tests automatically. It can be run as follows:

```python
main(['-vv'])
```

This line of code automatically discovers and runs the unit tests associated with the `arithmetic_arranger` function.

## Purpose

The purpose of the main file is to provide a simple way to test and verify the functionality of the `arithmetic_arranger` function. By importing the function and using it with different inputs, you can check how well it arranges and formats arithmetic problems. Additionally, the unit tests ensure that the function behaves correctly and adheres to the specified requirements.

## Development and Testing

When working on the `arithmetic_arranger` function or making changes to it, the main file can be used to quickly check its behavior with different inputs. By running unit tests, you can ensure that any modifications to the code do not introduce regressions and that the function continues to meet its intended purpose.

## Usage Example

```python
from arithmetic_arranger import arithmetic_arranger

# Example 1: Calling the function and printing the results without solutions
print(arithmetic_arranger(["32 + 698", "3801 - 2", "45 + 43", "123 + 49"]))

# Example 2: Running unit tests to validate the function's correctness
main(['-vv'])
```

This code can be used as a development tool to work with and test the `arithmetic_arranger` function efficiently.
