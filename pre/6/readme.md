https://github.com/hunter-teacher-cert/pre-acceptance-prework/blob/master/pre06.org

3,4,5 at
https://books.trinket.io/thinkjava/chapter7.html


Exercise 3  

In Exercise 9 we wrote a recursive version of power, which takes a double x and an integer n and returns xn. Now write an iterative method to perform the same calculation.


Exercise 4  

Section 6.7 presents a recursive method that computes the factorial function. Write an iterative version of factorial.


Exercise 5  

One way to calculate ex is to use the infinite series expansion:
ex = 1 + x + x2 / 2! + x3 / 3! + x4 / 4! + … 

The ith term in the series is xi / i!.

    Write a method called myexp that takes x and n as parameters and estimates ex by adding the first n terms of this series. You can use the factorial method from Section 6.7 or your iterative version from the previous exercise.

    You can make this method more efficient if you realize that the numerator of each term is the same as its predecessor multiplied by x, and the denominator is the same as its predecessor multiplied by i. Use this observation to eliminate the use of Math.pow and factorial, and check that you get the same result.
    Write a method called check that takes a parameter, x, and displays x, myexp(x), and Math.exp(x). The output should look something like:
    1.0     2.708333333333333     2.718281828459045

    You can use the escape sequence "\\t" to put a tab character between columns of a table.
    Vary the number of terms in the series (the second argument that check sends to myexp) and see the effect on the accuracy of the result. Adjust this value until the estimated value agrees with the correct answer when x is 1.
    Write a loop in main that invokes check with the values 0.1, 1.0, 10.0, and 100.0. How does the accuracy of the result vary as x varies? Compare the number of digits of agreement rather than the difference between the actual and estimated values.
    Add a loop in main that checks myexp with the values -0.1, -1.0, -10.0, and -100.0. Comment on the accuracy.
