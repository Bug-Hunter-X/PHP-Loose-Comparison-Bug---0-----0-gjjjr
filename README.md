# PHP Loose Comparison Bug

This repository demonstrates a common, yet subtle, bug in PHP related to loose comparisons using the `==` operator.  Loose comparison can lead to unexpected behavior when comparing values of different types, specifically when comparing strings and integers. 

The `bug.php` file shows the incorrect behavior using `==`, while `bugSolution.php` demonstrates the correct use of strict comparison (`===`).  Always prefer strict comparison (`===`) to avoid unintended type coercion and ensure accurate comparisons.

## How to Reproduce
1. Clone the repository.
2. Run `bug.php` using a PHP interpreter.
3. Observe the output.  Note that '0' and 0 are treated as equal.
4. Run `bugSolution.php`.
5. Observe the correct output where '0' and 0 are identified as unequal.

## Solution
Always use the strict comparison operator (`===`) when comparing values in PHP to avoid type juggling issues.