# Problems

## matching invoices

Our company has sent 400 invoices over the last few months. A company pays several invoices at the same time, without specifying which invoices.

Write a Python program to help solve the problem. 
1. The program should read the invoices directly from this repository using the url: https://github.com/rob4acre/problem_data/blob/8220bea41d6b574d5120eaf65a47821b3267c7bf/invoices.csv
2. The program should accept 2 input arguments. The total amount of the paid invoices and the name of the company
3. The program shall find the corresponding invoices from the company which add up to the given total
4. The list of matching invoices shall be output as a JSON formatted text file, with the amounts expressed as floats



## Satellite Coverage Planner

You are developing software for a company that controls and monitors satellites. Your company has been tasked with planning the coverage of a set of satellites over a linear region of the Earth's surface. The region is divided into a certain number of discrete sections (N), where each section can be covered by a satellite.

Each satellite has a limited coverage range, defined as an integer (K), and can cover K sections on either side of its current position. Satellites can be moved to any section, but each move takes time and resources, so the goal is to minimize the number of satellites necessary to cover all N sections.

You are given an array of integers, where each integer represents the number of sections that a specific satellite can cover.

Write a function:
```python
def min_satellites(coverage_ranges: List[int], num_sections: int) -> int:
    pass
```

Input:
* An array `coverage_ranges` of positive integers (1 <= coverage_ranges[i] <= 10^5), where each element is the coverage range of a satellite. The array can contain up to 100,000 elements.
* An integer `num_sections` (1 <= num_sections <= 10^9), the total number of sections that need to be covered.

Output:
* The function should return the minimum number of satellites that are needed to cover all `num_sections`. If it's not possible to cover all sections, return -1.

 Examples:
```python
assert min_satellites([1, 2, 3], 5) == 2
assert min_satellites([2, 2], 10) == -1
assert min_satellites([1, 2, 3, 4, 5], 20) == 4
```

 
