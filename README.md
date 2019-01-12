#CheckSum Validator
This is a project to create an algorithm for validating IDS against the Luhn formula
This problem is described in the book "Think Like a Programmer" by Anton Spraul as follows:

#The Luhn Formula: 
Using the original number, double the value of every other digit. Then add the values of the individual digits together. If a doubled value now has two digits, add the digits individually. The identification number is valid if the sum is divisible by 10. 
Write a program that takes an identification number of arbitrary length and determines whether the number is valid under the Luhn formula. The program must process each character before reading the next one.

#The Constraints:
I want to create a program that does the above, but can accept input of any length and will validate the ID number without knowing the whole number before the program starts running. In other words, I want the program to behave as if only one digit of the larger number is entered at a time rather than the entire number being passed to the algorithm together.

#Smaller Problems:
The larger design has the following smaller problems:
1) Knowing which digits to double
    The ID number digits will be entered from left to right like how we read numbers, but the digits to be doubled will be determined from right to left. How will we know which digits to double while receiving the digits in left to right order?
2) Adding individual digits when doubled digits become larger than 10  
    How will we add individual digits to our checksum, when the digit we double will become larger than 9 and need to have its associated digits added individually? What's the most efficient way?
3) End of Input
    How will we know when we've reached the end of the input and can complete the validation?

#Goals:
-Explain the problem-solving process throughout
-Implement solutions in multiple languages: C#, Java
-Understand the Time/Space Complexity of the solution and consider alternative methods/ how this problem could be solved with different constraints