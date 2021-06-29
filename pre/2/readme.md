https://github.com/hunter-teacher-cert/pre-acceptance-prework/blob/master/pre02.org

https://books.trinket.io/thinkjava/chapter2.html


Exercise 2  

The point of this exercise is (1) to use string concatenation to display values with different types (int and String), and (2) to practice developing programs gradually by adding a few statements at a time.

    Create a new program named Date.java. Copy or type in something like the hello world program and make sure you can compile and run it.
    Following the example in Section 2.4, write a program that creates variables named day, date, month, and year. The variable day will contain the day of the week (like Friday), and date will contain the day of the month (like the 13th). What type is each variable? Assign values to those variables that represent today’s date.
    Display (print out) the value of each variable on a line by itself. This is an intermediate step that is useful for checking that everything is working so far. Compile and run your program before moving on.
    Modify the program so that it displays the date in standard American format, for example: Thursday, July 16, 2015.
    Modify the program so it also displays the date in European format. The final output should be:
    American format:
    Thursday, July 16, 2015
    European format:
    Thursday 16 July 2015

Exercise 3  

The point of this exercise is to (1) use some of the arithmetic operators, and (2) start thinking about compound entities (like time of day) that are represented with multiple values.

    Create a new program called Time.java. From now on, we won’t remind you to start with a small, working program, but you should.
    Following the example program in Section 2.4, create variables named hour, minute, and second. Assign values that are roughly the current time. Use a 24-hour clock so that at 2pm the value of hour is 14.
    Make the program calculate and display the number of seconds since midnight.
    Calculate and display the number of seconds remaining in the day.
    Calculate and display the percentage of the day that has passed. You might run into problems when computing percentages with integers, so consider using floating-point.
    Change the values of hour, minute, and second to reflect the current time. Then write code to compute the elapsed time since you started working on this exercise.

Hint: You might want to use additional variables to hold values during the computation. Variables that are used in a computation but never displayed are sometimes called “intermediate” or “temporary” variables.


* * *

https://books.trinket.io/thinkjava/chapter3.html


3.12  Exercises

The code for this chapter is in the ch03 directory of ThinkJavaCode. See page ?? for instructions on how to download the repository. Before you start the exercises, we recommend that you compile and run the examples.

If you have not already read Appendix A.3, now might be a good time. It describes the command-line interface, which is a powerful and efficient way to interact with your computer.
Exercise 1   When you use printf, the Java compiler does not check your format string. See what happens if you try to display a value with type int using \%f. And what happens if you display a double using \%d? What if you use two format specifiers, but then only provide one value?
Exercise 2   Write a program that converts a temperature from Celsius to Fahrenheit. It should (1) prompt the user for input, (2) read a double value from the keyboard, (3) calculate the result, and (4) format the output to one decimal place. For example, it should display "24.0 C = 75.2 F".

Here is the formula. Be careful not to use integer division!
F = C × 	
9
5
	 + 32 
Exercise 3   Write a program that converts a total number of seconds to hours, minutes, and seconds. It should (1) prompt the user for input, (2) read an integer from the keyboard, (3) calculate the result, and (4) use printf to display the output. For example, "5000 seconds = 1 hours, 23 minutes, and 20 seconds".

Hint: Use the modulus operator.
Exercise 4   The goal of this exercise is to program a “Guess My Number” game. When it’s finished, it will work like this:
I'm thinking of a number between 1 and 100
(including both). Can you guess what it is?
Type a number: 45
Your guess is: 45
The number I was thinking of is: 14
You were off by: 31

To choose a random number, you can use the Random class in java.util. Here’s how it works:

Like the Scanner class we saw in this chapter, Random has to be imported before we can use it. And as we saw with Scanner, we have to use the new operator to create a Random (number generator).

Then we can use the method nextInt to generate a random number. In this example, the result of nextInt(100) will be between 0 and 99, including both. Adding 1 yields a number between 1 and 100, including both.

    The definition of GuessStarter is in a file called GuessStarter.java, in the directory called ch03, in the repository for this book.
    Compile and run this program.
    Modify the program to prompt the user, then use a Scanner to read a line of user input. Compile and test the program.
    Read the user input as an integer and display the result. Again, compile and test.
    Compute and display the difference between the user’s guess and the number that was generated.
