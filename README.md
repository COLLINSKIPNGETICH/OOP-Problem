# OOP-Problem

This project implements a function to generate a scoreboard for a competitive eating competition based on the amount of different food items consumed by each participant.

## Table of Contents

- [Description](#description)
- [Installation](#installation)

## Description

The function `calculate_score(participants)` takes a list of participant dictionaries as input, where each dictionary contains keys for 'name', 'chickenwings', 'hamburgers', and 'hotdogs', representing the participant's name and the quantity of each food item they consumed. It calculates the score for each participant based on the scoring criteria provided and returns a sorted scoreboard based on the scores. In case of tied scores, participants are sorted alphabetically by name.

## Installation

No installation is required. Simply include the `calculate_score` function in your Python project or script.

## Usage

To use the `calculate_score` function, import it into your Python script and pass a list of participant dictionaries to it as shown below:

```python
from scoreboard import calculate_score

participants = [
    {'name': "Habanero Hillary", 'chickenwings': 5, 'hamburgers': 17, 'hotdogs': 11},
    {'name': "Big Bob", 'chickenwings': 20, 'hamburgers': 4, 'hotdogs': 11}
]

scoreboard = calculate_score(participants)
print(scoreboard)
Example
python
Copy code
# Input
participants = [
    {'name': "Habanero Hillary", 'chickenwings': 5, 'hamburgers': 17, 'hotdogs': 11},
    {'name': "Big Bob", 'chickenwings': 20, 'hamburgers': 4, 'hotdogs': 11}
]

# Output
scoreboard = [
    {'name': "Big Bob", 'score': 134},
    {'name': "Habanero Hillary", 'score': 98}
]
Tests
This project includes test cases to ensure the correctness of the calculate_score function. To run the tests, execute the following command:

Copy code
python test_scoreboard.py
