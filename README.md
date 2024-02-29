Given a number N and N inputs containing two space- separated integers in each line, representing the Power Pl and Coefficient Ci of a polynomial. Write a program that prints the polynomial in the standard form of Cix^Pi + Ci-1x^Pi-1+....+ C1x + CO.

Input

.The first line of input contains an integer representing N that is the number of terms in the polynomial.

.The next N lines of input contain two space-separated integers in each line, representing the Power Pi and Coefficient Ci

Output

The output should be in the form of Cix^Pi + Ci-1x^Pi-1+....+ C1x + CO.

.If the coefficient is 0, then the term should not be printed.

.If the term with the highest power is negative, it should be represented as -Cix Pi

.If the term where power is 1, it should be represented as C1x instead of C1x^1.

.If the polynomial power is 0 and the constant term is also 0, then print to represent the polynomial.

.For term Cix Pi, if the coefficient of the term Ci is 1, then print x Pi instead of 1x Pi.

Constraints

.N is less than or equal to 100.

.Pi is greater than or equal to O and less than 1000.

.Ci is greater than or equal to -1000 and less than or equal to 1000.

Explanation

.For example, if the given number is N=4,

.For power, the coefficient is 5.

.5x^0 (The coefficient of x^0 is 5 and x^0 is equivalent to 1)

  .5*1=5
  
.For power 1, the coefficient is 0

  .Ox^1 (If the coefficient of x1 is 0 then the term should not be printed)

.For power 2, the coefficient is 10.

  .10x^2 (The coefficient of x^2 is 10)
  
.For power 3, the coefficient is 6.

  .6x^3 (The coefficient of x^3 is 6)
  
.The highest power of x is 3.

.The output should be 6x^3 + 10x^2 + 5.

For example, if the given number is N=6,

.For power 0, the coefficient is 7.

  .7x^0 (The coefficient of XO is 7 and x^0 is. equivalent to 1)
  
  .7*1=7
  
.For power 1, the coefficient is 3

   .3x (If the term with power 1, it should be represented as Cx instead of Cx^1.)
   
.For power 2, the coefficient is 0.

   .0x^2 (If the coefficient of x^2 is 0 then the term should not be printed)
   
.For power 3, the coefficient is 2.

   .-2x^3 (If the term with the highest power is negative, it should be represented as -Cix^Pi.)
   
For power 4, the coefficient is 1.

   . 1x^4 (The coefficient of x^4 is 1)
   
For power 5, the coefficient is 6.

   . 6x^5 (The coefficient of x^5 is 6)
   
The highest power of x is 5.

The output should be 6x^5 + x^4-2x^3+3x+7.

Sample Input

4

0 5

1 0

2 10

36

Sample Output

6x^3 + 18x^2 + 5
