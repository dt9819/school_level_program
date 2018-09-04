# School Level Logic Programs
I am Using Python to implement Logic Programming.

# Problem 1: Check if a number is Perfect Square
## Theory: 

### 1. Sum of the first n odd numbers is always a square. For example,
        1
        1 + 3 = 4
        1 + 3 + 5 = 9
        1 + 3 + 5 + 7 = 16
        ---------------------
        ------------------------
        
        So the standard formula gives us:

        sum_odd(n) = n(2a + (n-1)d)/2
                   = n(2 + (n-1)2)/2
                   = n(1 + n - 1)
                   = n^2
        But using standard formulae is annoying, so how about trying a little induction.

        sum_odd(1) = 1

        sum_odd(n+1) = sum_odd(n) + (2n + 1)
                     = n^2 + 2n + 1
                     = (n+1)^2

### 2. There are two rules to check if a number is perfect square or not
#### Rule 1: Unit digit shoul not be either of 2, 3, 7, 8
              For example: 254692 is not a perfect square because last digit is 2.
#### Rule 2: Digit Sum or digit root should either of these 1, 7, 4, 9
              For example: 125 => 1 + 2 + 5 => 8 is not a perfect square
                           100 => 1 + 0 + 0 => 1 is a perfect square
                           152364 => 1 + 5 + 2 + 3 + 6 + 4 => 21 => 2 + 1 => 3 is not a perfect square.
  
 - ![#f03c15](https://placehold.it/15/f03c15/000000?## Program to Check if a number is Perfect Square (implemented in Python)=+) `#f03c15` 
