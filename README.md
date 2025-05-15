<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2>How to declare variables in different ways in JavaScript?</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>In JavaScript, variables can be declared using keywords like var, let, or const, each keyword 
is used in some specific conditions. Understanding these declarations is crucial for managing 
variable lifetimes and avoiding unintended side effects in code.<?p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Table of Content</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<ul>
  <li>JavaScript var</li>
  <li>JavaScript let</li>
  <li>JavaScript const</li>
  <li>Difference Between var, let, and const</li>
</ul>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2>JavaScript <b><mark>var</mark></b></h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>This keyword is used to declare variables globally. If you use this keyword to declare a variable 
then the variable can be accessible globally and changeable also. It is good for a short length 
of codes, if the codes get huge then you will get confused.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Syntax:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>var variableName = "Variable-Value;"</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Example: This example shows the use of <b><mark>var</mark></b>.</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>
var geeks = "GeeksforGeeks";
console.log(geeks);
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Output:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>GeeksforGeeks</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2>JavaScript <b><mark>let</mark></b></h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>This keyword is used to declare variables locally. If you use this keyword to declare a 
variable then the variable can be accessible locally and it is changeable as well. It is good 
if the code gets huge.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Syntax:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>let variableName = "Variable-Value;"</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Example: This example shows the use of <b><mark>let</mark></b>.</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>
if (true) {
    let geeks = "GeeksforGeeks";
    console.log(geeks);
}

/* This will be error and 
   show geeks is not defined */
console.log(geeks);
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Output:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>GeeksforGeeks</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2>JavaScript <b><mark>const</mark></b></h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>This keyword is used to declare variable locally. If you use this keyword to declare a variable 
then the variable will only be accessible within that block similar to the variable defined by 
using let and difference between let and const is that the variables declared using const values 
can’t be reassigned. So we should assign the value while declaring the variable.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Syntax:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>const variableName = "Variable-Value;"</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Example: This example shows the use of <b><mark>const</mark></b>.</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>
1  const geeks = "GeeksforGeeks";
2  console.log(geeks);
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Output</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>GeeksforGeeks</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2>Difference Between var, let, and const</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

|  <b><mark>var</mark></b>  |  <b><mark>let</mark></b> |  <b><mark>const</mark></b> |
|:-----------------:|:--------------------:|:-------------------:|
|Can be redeclared	| Cannot be redeclared	| Cannot be redeclared |
|Can be reassigned a value |Can be reassigned a value|Cannot reassign the value |
|Only have global and function scope |Can have a block scope |Can have a block scope |
|Variables are hoisted on top and can be used anywhere | Variables must be initialized before use | Variables must be initialized before use |
|Can be redeclared anywhere in the program |	Cannot be redeclared inside a block	| Cannot be redeclared inside a block |


<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->


