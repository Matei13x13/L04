# Bug reports for exercise2.py

Line: 3
Problem: is_passing returns False for a grade of exactly 5, but the docstring says "True if the grade is 5 or more".
Example: is_passing(5) returns False, expected True.
Fix: return grade >= 5

Line: 13
Problem: clamp returns low when x is less than or equal to low, but the docstring says "x, limited to the range from low to high", and the current code uses min(x, low) which incorrectly limits below low. It should use min(x, high) and max(x, low).
Example: clamp(3, 1, 10) returns 1, expected 3 (since 3 is within [1,10], but the function incorrectly returns low due to wrong min call).
Fix: return max(low, min(x, high))
