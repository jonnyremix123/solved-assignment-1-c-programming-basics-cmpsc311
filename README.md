Download Link: https://assignmentchef.com/product/solved-assignment-1-c-programming-basics-cmpsc311
<br>
In this assignment you will write simple functions in C. The purpose of this assignment is to assess your basic programming skills. You should have no difficulty in completing this assignment. If you do experience difficulty, then you should take some time to brush up on programming.

Like all assignments in this class you are prohibited from copying any content from the Internet or discussing, sharing ideas, code, configuration, text or anything else or getting help from anyone in or outside of the class. Consulting online sources is acceptable, but under no circumstances should <em>anything </em>be copied. Failure to abide by this requirement will result dismissal from the class as described in our course syllabus.

Below are the files in this assignment and their descriptions:

<ol>

 <li>h: a header file with the <em>declarations </em>of the functions that you will implement.</li>

 <li>c: a source file in which you will implement the functions whose declarations appear in student.h. In other words, you will provide the <em>definitions </em>of the functions declared in student.h.</li>

 <li>h: a header file with the declarations of the functions that are identical to those defined in student.h except they are prefixed with ref . These are the reference functions against which your implementations will be tested.</li>

 <li>o: an object file that contains the reference implementations of the functions declared in reference.h. This is a binary file that contains compiled reference implementations of functions.</li>

 <li>c: unit tests for the functions that you will implement. Each unit test passes an input to your implementation of a function and to the reference implementation of the same function and compares the outputs. This file will compile into an executable, tester, which you will run to see if you pass the unit tests.</li>

 <li>Makefile: instructions for compiling and building tester used by the make utility.</li>

</ol>

You workflow will consist of (1) implementing functions by modifying student.c, (2) typing make to build the tester, and (3) running tester to see if you pass the unit tests, and repeating these three steps until you pass all the tests. Although you only need to edit student.c for successfully completing the assignment, you can modify any file you want if it helps you in some way. When testing your submission, however, we will use the original forms of all files except student.c.

Below are the functions you need to implement:

<ol>

 <li>largest: Takes an array of integers and the length of the array as input, and returns the largest integer in the array. You can assume that the input array contains at least one element.</li>

 <li>sum: Takes an array of integers and the length of the array as input, and returns the sum of the integers in the array.</li>

 <li>swap: Takes a pointer to two integers and swaps the values of integers.</li>

</ol>

1

<ol start="4">

 <li>rotate: Takes a pointer to three integers and rotates the values of integers. For example, if the inputs are pointers to integers a, b, and c, then after a call to rotate, c contains the value of b, b contains the value of a, and a contains the value of c.</li>

 <li>sort: Takes a pointer to an array of integers and the length of the array as input and sorts the array. That is, after a call to sort the contents of the array should be ordered in ascending order. You can implement any sorting algorithm you want but you have to implement the algorithm yourself—you cannot use sort functions from the standard C library. We recommend using something simple, such as <a href="https://en.wikipedia.org/wiki/Bubble_sort">Bubble sort</a> or <a href="https://en.wikipedia.org/wiki/Selection_sort">Selection sort.</a></li>

 <li>doubleprimes: Takes an array of integers and the length of the array as input and doubles every prime element of the array. For example, if the input array contains [1, 7, -2], then after a call to doubleprimes the array will contain [1, 14, -2].</li>

 <li>negatearmstrongs: Takes an array of integers and the length of the array as input and negates every element of the array that is an <a href="https://en.wikipedia.org/wiki/Narcissistic_number">Armstrong number.</a> An Armstrong number (also called a Narcissistic number) is a number that is equal to the sum of its digits each raised to the power of the number of digits. For example, 153 is an Armstrong number because it has 3 digits and 1<sup>3 </sup>+5<sup>3 </sup>+3<sup>3 </sup>=153. Thus, if an input array contains [2, -153, 153], then after a call to negatearmstrongs the array will contain [2, -153, -153].</li>

</ol>

You are encouraged to write helper functions to simplify the implementations of the above functions. You should, however, not use a library function and implement all helper functions yourself. For example, if you need a function to raise number <em>a </em>to power <em>b</em>, you should implement that function yourself.

2