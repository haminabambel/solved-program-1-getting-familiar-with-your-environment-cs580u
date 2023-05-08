Download Link: https://assignmentchef.com/product/solved-program-1-getting-familiar-with-your-environment-cs580u
<br>
<h3><u>Driver Code and Test Input Files</u></h3>

<h3>●     Driver Code</h3>

<ul>

 <li><a href="https://drive.google.com/file/d/0B5NpY9dM1zfBR2lGdTFtandQZVk/view?usp=sharing">c</a>

  <ul>

   <li><em>All of the function interfaces are provided for you. You just need to implement them. <strong>You must use the driver code as I have given you and only make alterations where stated. DO NOT change it to take user input, etc.</strong></em></li>

  </ul></li>

</ul>

<h3><u>Grading Rubric</u></h3>

<strong><em>TOTAL: 10 points</em></strong>

<h2>●     Part 1 (1 point):</h2>

<ul>

 <li>Compiles and outputs “hello world” when run: 1 point</li>

</ul>

<h2>●     Part 2 (8 points):</h2>

<ul>

 <li>Part A: 2 points</li>

 <li>Part B: 3 points</li>

 <li>Part C: 3 points</li>

</ul>

<h2>●     Style Guidelines (1 point)</h2>

<ul>

 <li>Follows requested program structure and submission format</li>

 <li>Follows <a href="https://drive.google.com/open?id=1PyRZpBay-PZ8CzQRDAaz2Oke0K0T1rIBHMKNzZWjgbI">formatting guidelines</a></li>

</ul>

<h3><u>Guidelines</u></h3>

This is an individual assignment. You must do the vast majority of the work on your own. It is permissible to consult with classmates to ask general questions about the assignment, to help discover and fix specific bugs, and to talk about high level approaches in general terms. It is not permissible to give or receive answers or solution details from fellow students.




You may research online for additional resources; however, you may not use code that was written specifically <em>to</em> solve the problem you have been given, and you may not have anyone else help you write the code or solve the problem. You may use code snippets found online, providing that they are appropriately and clearly cited, within your submitted code.




<em>By submitting this assignment, you agree that you have followed the above guidelines regarding collaboration and research.</em>




<em> </em>

<h1>Part 2 – Using Variables and Arithmetic</h1>




For the second part of the program we will be using variables and math. Helpful link: <a href="http://www.cplusplus.com/reference/cstdio/printf/">printf</a>

<h1>●    Part A</h1>




<ul>

 <li>Uncomment the remainder of the code, and add the following expressions shown here in the main:

  <ul>

   <li>3x<sup>3</sup> – 5x<sup>2</sup> + 6 for x = 2.5.</li>

   <li>The result of (4 × 10<sup>8</sup> + 2 × 10<sup>-7</sup>) / (7 × 10<sup>-6</sup> + 2 × 10<sup>8</sup>)

    <ul>

     <li>read the comments in the code to know where to write your code</li>

    </ul></li>

   <li>To round off an integer i to the next largest even multiple of another integer j, the following formula can be used:

    <ul>

     <li>int next_multiple = i + j – i % j

      <ul>

       <li>For example, to round off 256 days to the next largest number of days evenly divisible by a week, values of i = 256 and j = 7 can be substituted into the preceding formula as follows:<em>int next_multiple = 256 + 7 – 256 % 7 </em></li>

      </ul></li>

    </ul></li>

  </ul></li>

</ul>




<ul>

 <li>Write a function called findNextMultiple(int number1, int number2) to find the next largest even multiple for the following values of i and j:

  <ul>

   <li><strong><u>i  </u></strong><strong> <u>                j</u></strong><u></u>365                  712258              28996                  4</li>

  </ul></li>

</ul>




<ul>

 <li>Write a function, float convertFtoC(float fahrenheit), that converts 40° from degrees Fahrenheit (F) to degrees Celsius (C) using the following formula and returns the result:

  <ul>

   <li>C = (F – 32) / 1.8</li>

  </ul></li>

</ul>

<h1>●    Part B</h1>

<ul>

 <li>In the next part of the program we are going to see how choosing the wrong data types and careless casting can result in data loss. You should see inaccurate results.

  <ul>

   <li>Write functions to typecast a long integer to the following datatypes

    <ul>

     <li>int</li>

     <li>double</li>

     <li>char</li>

    </ul></li>

  </ul></li>

</ul>

<h1>●    Part C</h1>

<ul>

 <li>In the Fibonacci sequence, the first two Fibonacci numbers, called f0 and f1, are defined to be 0 and 1, respectively. Thereafter, each successive Fibonacci number f<em>i</em> is defined to be the sum of the two preceding Fibonacci numbers f<em>i</em>2 and f<em>i</em> So f<em>i</em>2 is calculated by adding together the values of f<em>i</em>0 and f<em>i</em>1.

  <ul>

   <li>Write a function that generates the first 20 Fibonacci numbers (including 0 and 1) using a loop.</li>

   <li>You should return the final resulting value</li>

  </ul></li>

</ul>







Part 3 – Submission




<ul>

 <li>Required code organization:

  <ul>

   <li><strong>&lt;user_id&gt;_program1.c</strong></li>

  </ul></li>

 <li>While inside your program1 folder, create a zip archive with the following command

  <ul>

   <li>zip -r <strong>&lt;user_id&gt;_program1</strong> <strong>&lt;user_id&gt;_program1.c</strong>

    <ul>

     <li>This creates an archive of all file and folders in the current directory called<strong> &lt;user_id&gt;_program1.zip</strong></li>

     <li><strong>Do not zip the folder itself, only the files required for the program</strong></li>

    </ul></li>

   <li>Upload the archive as specified for the course</li>

  </ul></li>

</ul>













#include&lt;stdio.h&gt;

#include &lt;math.h&gt;

#include &lt;assert.h&gt;




//Function to calcualte next multiple of two given values

int findNextMultiple(int number1, int number2){

//TODO

int next_multiple;

next_multiple = number1 + number2 – number1%number2;

printf(“Next Multiple of the number is: %d
”, next_multiple);

}




//Function to convert Fahrenheit to Celsuius

float convertFtoC(float fahrenheit){

//TODO

float Celsius;

Celsius = (fahrenheit – 32) / 1.8;

printf(“Temperature in Fahrenheit is: %f
”, Celsius);

}




//Function to calculate fibonacci series for first 20 numbers

int fibonacci(int n){

//TODO

int fib1=0, fib2=1;

int next_number;

if (n&lt;=1)

return n;

for (int i=1; i&lt;=n; i++)

{

printf(“%d “, fib2);

next_number = fib1 + fib2;

fib1 = fib2;

fib2 = next_number;

}




}




//Function to cast a long to an int

int castToInt(long num){

//TODO

}




//Function to cast a long to an double

double castToDouble(long num){

//TODO

}




//Function to cast a long to an char

char castToChar(long num){

//TODO

}




//The main driver

int main(){




//TODO Write code to print “Hello World”

printf(“tHello World
”);




//TODO For given value of x calculate value of expression

printf(“
t=============================
”);

printf(“t=           PART A          =
”);

printf(“t=============================

”);




printf(“
t=========Starting Expression Conversion Tests===========
”);

//Write code to evaluate the following expression: 3x^3 – 5x^2 + 6 for x = 2.5.




//float result = 0; //TODO write your expression here

double l,x,y;

x = 2.55;

float result = 3*pow(x,3) – 5*pow(x,2) + 6;

//assert(result == 21.625);

printf(“Value of the expression 3x^3-5x^2+6 for x(2.5) = %f
”, result);




//Write code to evaluate the following expression: (4 * 10^8 + 2 * 10^-7) / (7 * 10^-6 + 2 * 10^8)




//int result1 = 0;//TODO write your expression here

int result1 = (4*pow(10,8) + 2*pow(10,-7))/(7*pow(10,-6) + 2*pow(10,8));

//assert(result == 2.0);

printf(“Value of the expression (4 × 10^8 + 2 × 10^-7) / (7 × 10^-6 + 2 × 10^8) = %e”, result1);

printf(“
tt….Converting Expressions Tests Passed
”);




printf(“
t=========Starting Next Multiple Tests===========
”);

//For given numbers find next multiple

int number1 = 365, number2 = 7;

//assert(371 == findNextMultiple(number1,number2));

findNextMultiple(number1,number2);




number1 = 12258; number2 = 28;

//assert(12264 == findNextMultiple(number1,number2));

findNextMultiple(number1,number2);




number1 = 996; number2 = 4;

//assert(1000 == findNextMultiple(number1,number2));

findNextMultiple(number1,number2);

printf(“
tt….Next Multiple Tests Passed
”);




printf(“
t=========Starting Fahrenheit to Celsius Tests===========
”);




//Convert Fahrenheit value to Celsius value

float fahrenheit = 95;

float celsius = convertFtoC(fahrenheit);

//assert(35.0 == celsius);




fahrenheit = 32;

celsius = convertFtoC(fahrenheit);

//assert(0.0 == celsius);




fahrenheit = -40;

celsius = convertFtoC(fahrenheit);

//assert(-40.0 == celsius);

printf(“
tt….Fahrenheit to Celsius Tests Passed
”);




printf(“
t=============================
”);

printf(“t=           PART B          =
”);

printf(“t=============================

”);










printf(“
t=============================
”);

printf(“t=           PART C          =
”);

printf(“t=============================

”);




printf(“
t=========Starting Fibonacci Tests===========
”);

//finding fibonacci series for first 20 numbers

printf(“%d”, fibonacci(20));




//assert(4181 == fibonacci());




printf(“
tt….Fibonacci Tests Passed
”);




printf(“
t=========ALL TESTS PASSED===========
”);




return 0;

}