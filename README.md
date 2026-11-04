# Simulated Device Monitoring and Alert System

Student Name: John Michael M. Beig
Student Number: 2601277
Section: 1CPE-C

# Project Description
This program monitors simulated device temperature readings. It stores the readings in a list, accepts new valid readings, and classifies each reading as NORMAL, WARNING, or CRITICAL. It then prints a numerical summary and the overall monitoring status. It was written for CPP102 Week 17 using only Python built-in features.

# Features
- View all stored temperature readings
- Add a new reading (whole numbers from 0 to 100 only)
- Classify every reading (below 30 is NORMAL, 30 to 35 is WARNING, above 35 is CRITICAL)
- Generate a summary: count, total, average, minimum, maximum, category counts and percentages, and overall status
- Reject invalid menu choices and invalid readings without crashing

# Requirements
- Python 3 (no external packages)

# How to Run
1. Open a terminal inside the Week17 folder.
2. Type: python device_monitor.py
   (On macOS or Linux, type: python3 device_monitor.py)

## Sample Output
```
MONITORING SUMMARY
------------------
Number of readings  : 5
Total of readings   : 160
Average temperature : 32.00 °C
Minimum temperature : 28 °C
Maximum temperature : 37 °C

NORMAL   : 2 (40.00%)
WARNING  : 2 (40.00%)
CRITICAL : 1 (20.00%)

Overall Status: ATTENTION REQUIRED
```

## Test Cases
I performed 16 tests. 16 passed and 0 failed. Full details are in [test_cases.md](test_cases.md).

## Known Limitations
- Readings are lost when the program closes, because file handling is not used.
- Readings cannot be edited or deleted once they are added.
- Only whole-number readings from 0 to 100 are accepted.
- The temperature limits are for this classroom simulation only. They are not real device-safety standards.

## Reflection
Working on the Simulated Device Monitoring and Alert System taught me how a list of numbers can support a real decision by classifying readings as NORMAL, WARNING, or CRITICAL. The hardest part was input validation, so I used loops with try and except to reject bad input without crashing. Writing 16 test cases showed me that testing is a habit, not just a final step. In the future, I would like to add file saving and edit and delete options.
