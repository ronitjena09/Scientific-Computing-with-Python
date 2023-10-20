# Time Calculator

The main file, `main.py`, serves as an entry point for running and testing the time calculator program provided by the `time_calculator` module. This program allows you to add a duration to a given starting time and calculate the resulting time in both 12-hour and 24-hour formats. Additionally, if a starting date is provided, the program can calculate the new date based on the duration and the day of the week. Below, you will find an explanation of how to use the main file and how to run unit tests to ensure that the time calculator functions correctly.

## Usage

### Importing the `add_time` Function

```python
from time_calculator import add_time
from unittest import main
```

The main file begins by importing the `add_time` function from the `time_calculator` module. This function allows you to calculate the new time based on a starting time and a duration.

### Calculating New Time

You can use the `add_time` function to calculate the new time. Here's an example:

```python
new_time = add_time("11:06 PM", "2:02")
```

In this example, the function is used to add a duration of 2 hours and 2 minutes to a starting time of "11:06 PM." The result is stored in the `new_time` variable.

### Printing the Result

You can print the result to see the calculated time:

```python
print(new_time)
```

This code will display the new time in both 12-hour and 24-hour formats.

### Running Unit Tests

To verify the correctness of the time calculator function, the main file utilizes the `unittest` framework to run unit tests automatically. You can run the tests using the following line of code:

```python
main(module='test_module', exit=False)
```

This line of code automatically discovers and runs the unit tests associated with the `time_calculator` module.

## Purpose

The main file is designed to showcase how to use the time calculator program to add a duration to a starting time and calculate the resulting time. It also demonstrates the ability to include a starting date to calculate the new date based on the duration and the day of the week.

## Development and Testing

During development, the main file allows you to test and verify the functionality of the time calculator. You can experiment with different starting times and durations and observe the calculated results. Additionally, running unit tests ensures the accuracy of the time calculations.

## Usage Example

```python
from time_calculator import add_time
from unittest import main

print(add_time("11:06 PM", "2:02"))

main(module='test_module', exit=False)
```

This code demonstrates how to use the time calculator program to add a duration to a starting time and calculate the resulting time. Additionally, it includes unit tests to ensure the accuracy of the time calculations.
