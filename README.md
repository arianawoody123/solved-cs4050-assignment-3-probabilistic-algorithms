Download Link: https://assignmentchef.com/product/solved-cs4050-assignment-3-probabilistic-algorithms
<br>



<ol>

 <li><strong>Computing Π (Pi) probablistically</strong></li>

</ol>

Think of a square, with sides = 2, centered at the origin with a circle inscribed within the square. If you throw N darts that land in the square, some of them, M, will land inside of the circle. Since the area of the circle is Πr<sup>2</sup> ( which is Π since r = 1) and the area of the square is 4, the ratio of the circle’s area to the square’s area is Π/4. M/N should approximate Π/4, so 4M/N should approximate Π.

Simulate the throwing of the darts and printout the approximate value of Π computed for various iterations such as 1000, 10,000, 100,000, 1,000,000 and 100,000,000 (if time allows (it should)).

<ol start="2">

 <li><strong>Testing for Prime Numbers</strong></li>

</ol>

You can test if a number P is a prime by checking to make sure P % n (n is an integer) is not zero for lots of values 1 &lt; n &lt; P. Write a program to input a number (or generate a number randomly) and test it against k random values. Pick a bunch of known composite numbers and see how accurately your program rejects them. See if the results improve for larger values of k. Try k = 10, 100, 1000 and 10,000. You can easily try the program against large composite numbers by including: i. Even numbers

<ol>

 <li>Numbers whose final digit is a 5</li>

</ol>

<ul>

 <li>Numbers where the sum of the digits is divisible by 3. iv. Number constructed as the product of two positive integers.</li>

</ul>

<ol>

 <li>Randomly generated numbers X that are then adjusted as follows: X = X – X%K &lt;– X will now be divisible by K.</li>

</ol>

<ol start="3">

 <li><strong>Searching an Array</strong></li>

</ol>

Create an array of 1000 ints. Search for a value known to be in the array by generating an index at random and testing to see if the searched for int is in the array at that index. Write your program to make at most 5000 guesses. Try 100 different searches and compute the average number of comparisons the program has to do. You can easily pick a target by randomly selecting a value from the array.

<ol start="4">

 <li><strong>Monte Carlo Integration</strong></li>

</ol>

For this problem, you are to determine the approximate integral of a function on an interval two different ways using probabilities.

<strong>   Dart throwing:</strong> Construct a rectangular region around the function. Pick random points in the rectangle. Find the percentage of these that are in the area under the function. The area under the function (the function’s integral on this region) can be found by multiplying this percentage by the rectangle’s area.

<strong>   Mean of values at random locations:</strong> Compute the mean value of the function at random locations in the interval and multiply this value by the interval’s width.

Compare these two methods to the trapezoid method. Compare both acccuracy and running times. Make sure to use interesting functions for your tests.

<ol start="5">

 <li><strong>8 queens problem</strong></li>

</ol>

Solve the 8 queens problem by gluing k random queens to the board and placing the other 8-k queens using backtracking. What value for k gives the best result (on avereage)? How does the running time compare to the traditional backtracking algorithm