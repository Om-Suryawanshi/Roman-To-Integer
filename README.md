# Roman-To-Integer

Theory 

I -            1,
V  -           5,
X   -          10,
L     -        50,
C       -      100,
D         -    500,
M           -  1000.


2 is written as II in Roman numeral, just two one's added together. 12 is written as XII, which is simply X + II. The number 27 is written as XXVII, which is XX + V + II.

# Special Cases

I can be placed before V (5) and X (10) to make 4 and 9. 
X can be placed before L (50) and C (100) to make 40 and 90. 
C can be placed before D (500) and M (1000) to make 400 and 900.

Here's a breakdown of how the code works:

1. A dictionary roman is defined, which maps each Roman numeral character to its corresponding decimal value.

2. The variable result is initialized to 0, which will store the accumulated decimal value.

3. The code then iterates over each character in the input string s using a for loop.

4. Inside the loop, it checks if the current character (s[i]) is smaller than the next character (s[i + 1]). If this condition is true, it means that the current character represents a subtractive form (e.g., IV for 4, IX for 9). In this case, the decimal value corresponding to the current character is subtracted from the result.

5. If the condition in step 4 is not true, it means that the current character represents an additive form (e.g., III for 3, XVII for 17). In this case, the decimal value corresponding to the current character is added to the result.

6. After iterating through all the characters in the input string, the final result is returned.
