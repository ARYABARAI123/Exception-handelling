# Exception-handelling
## Overview
This Java program serves as a versatile calculator, capable of performing both arithmetic and statistical operations. It includes features for user input handling, arithmetic calculations (addition, subtraction, multiplication, division, and exponentiation), and statistical calculations (mean, variance, and standard deviation).

The program employs exception handling to address potential errors, such as invalid input or unsupported operations during user input and calculations. It catches InputMismatchException for invalid input and IllegalArgumentException for unsupported operations, providing informative error messages to the user.

## Contents
RationalCalculator.java
knl.java
exceptionhandelling.java
java class is the entry point for the calculator program. It initializes instances of UserInput and Calculator to handle user input and perform calculations, respectively. The program prompts users to choose between arithmetic and statistical operations, then guides them through the process, displaying results accordingly. Exception handling is implemented to address input mismatch and illegal argument issues.

## Methods
main(String[] args)
 Description: Initiates the calculator program by handling user input, choosing the type of operation, and performing the selected operation.
 printArray(double[] array)
 Description: Utility method to print an array of double values.
## Calculator.java
 The Calculator.java class contains methods to perform various arithmetic and statistical operations. It includes methods for addition, subtraction, multiplication, division, exponentiation, mean, variance, and standard deviation. The class utilizes the Arrays class for statistical calculations.

## Methods
## Arithmetic Operations
### add(double n1, double n2): Adds two numbers.
### subtract(double n1, double n2): Subtracts the second number from the first.
### multiply(double n1, double n2): Multiplies two numbers.
### divide(double n1, double n2): Divides the first number by the second.
### sqrt(double n): Calculates the square root of a number.
### power(double n1, double n2): Raises the first number to the power of the second.
## Statistical Operations
### mean(double[] arr): Calculates the mean (average) of an array of numbers.
### variance(double[] arr): Calculates the variance of an array of numbers.
### stddev(double[] arr): Calculates the standard deviation of an array of numbers.
## UserInput.java
The UserInput.java class manages user input for the calculator program. It includes methods to obtain integer, double, string, and array inputs from the user. The class utilizes the Scanner class for input reading.

## Methods
 getScanner()
 Description: Returns a Scanner object for reading input.
getIntInput(String message)
 Description: Gets an integer input from the user with a specified prompt message.
getDoubleInput(String message)
 Description: Gets a double input from the user with a specified prompt message.
getStringInput(String message)
 Description: Gets a string input from the user with a specified prompt message.
getArrayInput()
 Description: Gets an array input from the user by specifying the size and entering elements.

# Exception Handling 
## Classes Used:
FactorialException: This is a custom exception class used to handle invalid input for calculating factorial. It extends the Exception class and overrides the toString() method to display the error message along with the incorrect input number.

NOMATCHEXCP: Another custom exception class used to handle cases where the input string doesn't match the expected value. It also extends the Exception class and overrides the toString() method to provide detailed error messages.

ExceptionDemo: This is the main class of the program. It contains the main method where the exception handling logic is implemented. It also includes a method to calculate factorial (factorial) and demonstrates the usage of both custom and built-in exceptions.

## Methods Used:
main: This method is the entry point of the program. It handles command-line arguments, performs factorial calculations, and accepts user input to demonstrate exception handling.

factorial: This method calculates the factorial of a given integer recursively.

## Usage:
Compile the program using javac ExceptionDemo.java.

Run the program using java ExceptionDemo <arguments> where <arguments> are integers separated by spaces.

Follow the instructions to input a string and observe how exceptions are handled.

This program demonstrates the use of custom exceptions (FactorialException and NOMATCHEXCP) along with built-in exceptions (NumberFormatException). It showcases how to handle various types of exceptions gracefully in a Java program.
