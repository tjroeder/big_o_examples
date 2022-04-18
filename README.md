# Big O

This repository contains 4 solutions to the same problem. Two of the examples are written in Javascript and two are written in Ruby.

## Problem

Given an array of numbers, check if there are any duplicates

## Analysis Questions
### Example 1
* For the input `test_case_1`, how many times does the `containsDuplicate` method make the comparison between `num_1` and `num_2`? What about for `test_case_2`?
  * It makes the comparison 6 times. It makes the comparison 16 times. 
* Let's say the algorithm is given an input array with a million numbers. What is the *least* number of comparisons the algorithm could make between `num_1` and `num_2`? What would have to be true about that array?
  * It would make two comparisons in the best case scenario. The second element would be the same as the first.
* If the input array has `n` elements, what is the *most* number of comparisons the method would make as a **function** of `n`?
  * `n^2` if there are no matches.
* Does this algorithm create any new data structures that are roughly the same size as the input array? For example another array or Hash/Object?
  * No.

### Example 2
* For the input `test_case_1`, how many times does the `containsDuplicate` method make the comparison between `num_1` and `num_2`? What about for `test_case_2`?
  * It makes the comparison 9 times for test case 1. It takes 7 times for test case 2.
* Let's say the algorithm is given an input array with a million numbers. What is the *least* number of comparisons the algorithm could make between `num_1` and `num_2`? What would have to be true about that array?
  * It would make one iteration through n, than at minimum 1 comparisons. The second element would be the same as the first.
* If the input array has `n` elements, what is the *most* number of comparisons the method would make as a **function** of `n`?
  * `2n` which can be reduced to `O(N)` due to removal of least significant terms.
* Does this algorithm create any new data structures that are roughly the same size as the input array? For example another array or Hash/Object?
  * Yes, there it a Hash created in the first iteration.
## Exercise

Analyze the code for example_1 (.js or .rb whichever you prefer). Start by running the code for different test cases and understanding the algorithm. Then, answer the Analysis Questions above.

When you are ready, repeat the process for example_2.

## THE Question

After you have completed the exercise for both examples, answer this question:

**Which algorithm is better?**
It depends on what is more important, space or time. Or if you have a little more information about the collection N, it could change which is best.
Example 1 is best if you are solving for space complexity.
Example 2 is best if you are solving for time complexity. 
