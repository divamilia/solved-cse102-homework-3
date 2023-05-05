Download Link: https://assignmentchef.com/product/solved-cse102-homework-3
<br>
You are going to write a complete C program which implements the following functionality:

<ul>

 <li>Your program will read two input files:</li>

</ul>

<strong>– </strong>values.txt <strong>– </strong>polynomial.txt

<ul>

 <li>Your program will create a file: <strong>– </strong>txt</li>

 <li>Your program will evaluate the same polynomial for each value read from <sub>txt </sub>and write the results to evaluations.txt</li>

</ul>

<h1>values.txt</h1>

This file holds double numbers separated by whitespace.

12.5 5 67.89 -6 -13.37

There may be as many as <sub>100 </sub>double numbers in this file. <strong>polynomial.txt</strong>

This file holds a polynomial in a character array form.

5x+23.5x^3-x^2

There will only be one polynomial expression. monomials are not ordered according to the powers of the variable x. The coefficient of x at each monomial is written before the character <sub>x</sub>. Powers of x is represented by character <sub>ˆ </sub>followed by a number. Each monomial will certainly include a character <sub>x</sub>. The length of a polynomial expression can reach up to <sub>1000 </sub>characters. <strong>evaluations.txt </strong>This file will hold the results of polynomial evaluations for each value read from <sub>values.txt</sub>. If your polynomial string is <sub>5x+23.5xˆ3-xˆ2</sub>, set <sub>x </sub>to be the value(one of the numbers read from values.txt) and evaluate the mathematical expression: <sub>evaluation = 5*x + 23.5*x*x*x – x*x</sub>. For the given example above, evaluations.txt will be as follows:

45804.69

2937.50

7349081.25

-5142.00

-56410.13

<strong>Remarks:</strong>

<ul>

 <li>In order to convert char arrays to numbers, you can use function <sub>sscanf() </sub>which is defined in <sub>&lt;stdio.h&gt;</sub>. For example:</li>

</ul>

double d1,d2; char a[] = “12.5 63.4” sscanf(a, “%lf%lf”, &amp;d1, &amp;d2);

<em>/* d1 stores 12.5 and d2 stores 63.4 */</em>

<ul>

 <li>In order to find powers of a number, you can use <sub>pow() </sub>function defined in <sub>&lt;math.h&gt;</sub></li>

</ul>

<strong>Turn in:</strong>

<ul>

 <li>Source code of a complete C program. Name of the file should be in this format: <sub>&lt;full_name&gt;_&lt;id&gt;.c</sub>.</li>

 <li>Example: <sub>c</sub>. Please do not use any Turkish special characters.</li>

 <li>You don’t need to use an IDE for this assignment. Your code will be compiled and run in a command window.</li>

 <li>Your code will be compiled and tested on a Linux machine(Ubuntu). GCC will be used.</li>

 <li>Make sure that your program does not require specific encodings/markings/line-ending-chars. Make sure it works with a file created in a linux environment.</li>

 <li>Make sure you don’t get compile errors when you issue this command : <sub>gcc &lt;full_name&gt;_&lt;id&gt;.c</sub>.</li>

 <li>A script will be used in order to check the correctness of your results. So, be careful not to violate the expected output format.</li>

 <li>Provide comments unless you are not interested in partial credit. (If I cannot easily understand your design, you may loose points.)</li>

 <li>You may not get full credit if your implementation contradicts with the statements in this document.</li>

</ul>