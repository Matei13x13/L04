# Bug reports for exercise1.py

Line: 3
Problem: is_even returns True for odd numbers (like 1, 3, 5) but the docstring says "true for even numbers". The condition uses == 1 instead of == 0.
Example: is_even(2) returns False, expected True.
Fix: return n % 2 == 0

Line: 8
Problem: rectangle_area returns the sum of width and height, but the docstring says "area of a rectangle", which should be width times height.
Example: rectangle_area(3, 4) returns 7, expected 12.
Fix: return width * height

Line: 12
Problem: double returns n + 2, but the docstring says "twice the number n", which means n * 2.
Example: double(5) returns 7, expected 10.
Fix: return n * 2
