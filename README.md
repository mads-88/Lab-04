# Lab 04 - SOP/POS and KMaps
# Austin Maples & Madison Hickey
# Team 48

In this lab, you’ve learned how to apply KMaps, Sum Of Products and Products of
sums to simplify digital logic equations. Then, you’ve proven out that they work
using an implemented design on your Basys3 boards.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Lab Summary

In this lab we used SOP and POS equations to simplify the truth table that was provided. We then coded
our equations into vivado. We then demonstrated these equations on our Basys3 board which translated our equations properly.

## Lab Questions

### Why are the groups of 1’s (or 0’s) that we select in the KMap able to go across edges?
They are able to go across the edges because the last rows and columns of bits only differ by one; making them adjacent and able to be grouped.

### Why are the names Sum of Products and Products of Sums?
Sum of Products is OR-ing (adding) groups of AND terms (products) to create an expression that makes the output 1. Product of Sums is AND-ing (multiplying) groups of OR terms (sums) to create an expression that forces the output 0

### Open the test.v file – how are we able to check that the signals match using XOR?
We use XOR to compare signals because XOR outputs 0 when both inputs are the same and 1 when they are different. By XOR-ing the outputs of each implementation, we can detect mismatches. If the result stays 0, all signals match; if it becomes 1, at least one output is different.
