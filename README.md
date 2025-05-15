<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h1>webdev with Geeks4Geeks</h1>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2>Web Development with Geeks 4 Geeks</h2>
<ol>
  <li><h3><a href="#01">What are var, let, const?</a></h3></li>
  <li><h3><a href="#02">Create Web Search utility,</a>,</h3></li>
  <li><h3><a href="#03">Make a map in HTML</a>,</h3></li>
</ol>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="01">01. How to declare variables in different ways in JavaScript?</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>In JavaScript, variables can be declared using keywords like <b><mark>var</mark></b>, 
<b><mark>let</mark></b>, or <b><mark>const</mark></b>, each keyword is used in some specific 
conditions. Understanding these declarations is crucial for managing variable lifetimes and 
avoiding unintended side effects in code.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Table of Content</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<ul>
  <li>JavaScript <b><mark>var</mark></b></li>
  <li>JavaScript <b><mark>let</mark></b></li>
  <li>JavaScript <b><mark>const</mark></b></li>
  <li>Difference Between <b><mark>var</mark></b>, <b><mark>let</mark></b>, and <b><mark>const</mark></b></li>
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
<h2>Difference Between <b><mark>var</mark></b>, <b><mark>let</mark></b>, and <b><mark>const</mark></b></h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

|  <b><mark>var</mark></b>  |  <b><mark>let</mark></b> |  <b><mark>const</mark></b> |
|:-----------------:|:--------------------:|:-------------------:|
|Can be redeclared    | Cannot be redeclared    | Cannot be redeclared |
|Can be reassigned a value |Can be reassigned a value|Cannot reassign the value |
|Only have global and function <b><mark>scope</mark></b> |Can have a <b><mark>block scope</mark></b> |Can have a <b><mark>block scope</mark></b> |
|Variables are <b><mark>hoisted</mark></b> on top and can be used anywhere | Variables must be initialized before use | Variables must be initialized before use |
|Can be redeclared anywhere in the program |    Cannot be redeclared inside a block    | Cannot be redeclared inside a block |

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="02">02. Search Bar using HTML, CSS and JavaScript</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>Every website needs a search bar through which a user can search the content of their 
concern on that page. We’re going to learn how to create one using only HTML, CSS, and 
JavaScript. Instead of getting into complex algorithms for finding related content, we’ll 
focus on a basic task—searching for specific words or phrases within text.</p>
<!-- image-search-01.png -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 01. search image ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center" width="100%">
  <img src="./images/image-search-01.png"
  title="Search image."
  alt="Search image"
  style="border: 2px solid #000000; width:35%;" />
</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Approach</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<ul>
  <li>Create HTML with a search input and an ordered list of animals.</li>
  <li>Now assign the relevant IDs and classes to particular input boxes and list items.</li>
  <li>Apply initial styles for the container, search bar, and list items. Consider animations or transitions for visual appeal.</li>
  <li>Write a function (search_animal()) to handle input, loop through items, and toggle display based on content match.</li>
</ul>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Example: In this example, we will see the implementation of the above search bar with HTML and with an example.</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>HTML</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>
&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;
&lt;head&gt;
    &lt;meta charset="UTF-8"&gt;
    &lt;meta name="viewport" 
          content="width=device-width, initial-scale=1.0"&gt;
    &lt;title&gt;Search Bar Example&lt;/title&gt;
    &lt;link rel="stylesheet" 
          type="text/css" href="./style.css"&gt;
&lt;/head&gt;
&lt;body&gt;
  &lt;div class="container"&gt;
    &lt;input id="searchbar" 
      onkeyup="search_animal()" 
      type="text" name="search" 
      placeholder="Search animals.."&gt;
    &lt;ul id='list'&gt;
      &lt;li class="animals"&gt;Cat&lt;/li&gt;
      &lt;li class="animals"&gt;Dog&lt;/li&gt;
      &lt;li class="animals"&gt;Elephant&lt;/li&gt;
      &lt;li class="animals"&gt;Fish&lt;/li&gt;
      &lt;li class="animals"&gt;Gorilla&lt;/li&gt;
      &lt;li class="animals"&gt;Monkey&lt;/li&gt;
      &lt;li class="animals"&gt;Turtle&lt;/li&gt;
      &lt;li class="animals"&gt;Whale&lt;/li&gt;
      &lt;li class="animals"&gt;Alligator&lt;/li&gt;
      &lt;li class="animals"&gt;Donkey&lt;/li&gt;
      &lt;li class="animals"&gt;Horse&lt;/li&gt;
    &lt;/ul&gt;
  &lt;/div&gt;
  &lt;script src="./script.js"&gt;&lt;/script&gt;
&lt;/body&gt;
&lt;/html&gt;
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>CSS</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 20px;
}
#searchbar {
  margin: 10px;
  padding: 10px;
  border-radius: 5px;
  width: 50%;
  box-sizing: border-box;
}
#list {
  list-style: none;
  padding: 0;
  margin: 0;
}
.animals {
  font-size: 1.2em;
  padding: 10px;
  border-bottom: 1px solid #ccc;
  animation: fadeIn 0.5s ease-in-out;
}
.animals:last-child {
  border-bottom: none;
}
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>JavaScript</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>
// JavaScript code
function search_animal() {
  let input = document.getElementById('searchbar').value
  input = input.toLowerCase();
  let x = document.getElementsByClassName('animals');
  for (i = 0; i < x.length; i++) {
    if (!x[i].innerHTML.toLowerCase().includes(input)) {
      x[i].style.display = "none";
    }
    else {
      x[i].style.display = "list-item";
    }
  }
}
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Output:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 02. search image ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center" width="100%">
  <img src="./images/image-search-02.gif"
  title="Search image."
  alt="Search image"
  style="border: 2px solid #000000; width:35%;" />
</p>
<!-- image-search-02.gif -->
<p>JavaScript is best known for web page development but it is also used in a variety of non-browser 
environments. You can learn JavaScript from the ground up by following this 
<a href="https://www.geeksforgeeks.org/javascript-tutorial/">JavaScript Tutorial</a> and 
<a href="https://www.geeksforgeeks.org/javascript-examples/">JavaScript Examples</a>.</p>

<p>HTML is the foundation of webpages, is used for webpage development by structuring websites 
and web apps. You can learn HTML from the ground up by following 
<a href="https://www.geeksforgeeks.org/html-tutorials/">this HTML Tutorial</a> and 
<a href="">HTML Examples</a>.</p>

<p>CSS is the foundation of webpages, is used for webpage development by styling websites 
and web apps. You can learn CSS from the ground up by following 
<a href="https://www.geeksforgeeks.org/css-tutorials/">this CSS Tutorial</a> and 
<a href="https://www.geeksforgeeks.org/css-examples/">CSS Examples</a>.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="03">03. How to Add Map in HTML?</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>When building websites, including a map is often necessary to display important locations, 
such as office addresses, at the footer or on dedicated pages. Adding a map enhances user 
experience, making it easier for users to locate your business or other important points 
of interest.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Prerequisites</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>Basic knowledge of HTML and CSS is required to follow along with the examples.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Methods to Add a Map in HTML</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>Now, let's explore two popular approaches for adding maps to a webpage:</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Table of Content</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<ul>
  <li>Methods to Add a Map in HTML
    <ul>
	  <li>Using &lt;iframe&gt; to Embed Google Maps</li>
      <li>Using Leaflet.js to Add Interactive Maps</li>
	</ul>
  </li>
</ul>
<p>Now we will learn one by one how we can add maps in HTML.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3>1. Using &lt;iframe&gt; to Embed Google Maps</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>The easiest and most commonly used method to add a map in HTML is by embedding a Google 
Map using the <iframe> tag. Google Maps provides an option to generate an embed code that 
you can copy and paste directly into your HTML document.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Steps to Embed Google Maps:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<ol>
  <li>Go to Google Maps.</li>
  <li>Search for the location you want to display.</li>
  <li>Click the Share option and choose Embed a Map.</li>
  <li>Copy the provided &lt;iframe&gt; code and paste it into your HTML where you want the map to appear.</li>
</ol>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Syntax:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>
&lt;iframe src="https://www.google.com/maps/embed?pb=YourMapURL"
    width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"&gt;
&lt;/iframe&gt;
</pre>
<h4>Example: Below given example demonstrates how to embed a goggle map into a webpage 
using an &lt;iframe&gt; element. It shows a webpage with centered heading and a google map 
showing specific location.</h4>

```
<!-- Using iframe -->
<!DOCTYPE html>
<html>

<head>
    <title>Embed Google Map</title>
</head>

<body style="display: grid;
 justify-content: center">
    <h2 style="text-align: center">
        Add map in html using iframe</h2>
    <iframe src="https://www.google.com/maps/embed?pb
    =!1m18!1m12!1m3!1d4291.745453141256!2d
    77.39914006293347!3d28.504393188935435!
    2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1
    !3m3!1m2!1s0x390ce626851f7009%3A0x62118
    5133cfd1ad1!2sGeeksforGeeks%20%7C%20
    Coding%20Classes%20%7C%20Noida!5e0!3m2!1
    sen!2sin!4v1725395799894!5m2!1sen!2sin" width="600" height="450" style="border: 0" allowfullscreen=""
        loading="lazy" referrerpolicy="no-referrer-when-downgrade">
    </iframe>
</body>

</html>
```

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Output:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 01. map image ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center" width="100%">
  <img src="./images/image-map-01.png"
  title="Map image 1."
  alt="Map image 1"
  style="border: 2px solid #000000; width:35%;" />
</p>
<!-- image-map01.jpg -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3>2. Using <b><mark>Leaflet.js</mark></b> to Add Interactive Maps</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p><b><mark>Leaflet</mark></b> is a popular open source library to add interactive maps in our website. It is a 
Javascript library for mobile friendly lighweight and interactive maps. It is designed to 
be easy to use and mobile-friendly.It is customizable, as you can customize it with variety 
of additional plugins.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Steps to Use <b><mark>Leaflet.js</mark></b>:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<ol>
  <li>Include the <b><mark>Leaflet.js</mark></b> library: Link the CSS and JavaScript files in your HTML document.</li>
  <li>Create a map container: Add a &lt;div&gt; element where the map will be displayed.</li>
  <li>Initialize the map: Use <b><mark>Leaflet.js</mark></b> to create the map and set the center coordinates and zoom level.</li>
</ol>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Syntax:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>
let map = L.map('map').setView([Latitude, Longitude], ZoomLevel);

L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
}).addTo(map);

L.marker([Latitude, Longitude]).addTo(map)
    .bindPopup('Popup Text Here.')
    .openPopup();
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Example: Below is the example for creating interactive map in our website using 
<b><mark>leaflet.js</mark></b>, it is a open-source javascript library. The map centers on India Gate, 
New Delhi and displays it with marker.</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

```
<!-- Using leaflet Map -->
<!DOCTYPE html>
<html>

<head>
    <title>Leaflet Map Example</title>
    <link rel="stylesheet" href="
    https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZy
    oHS5obTRR9BMY=" crossorigin="" />
    <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9V
        M+kNiyxNV1lvTlZBo=" crossorigin=""></script>
</head>

<body>
    <h2 style="text-align: center;">
        India Gate Location</h2>
    <div id="mapid" style="height: 75vh; width: 50vw;
     margin-left: 25%;"></div>
    <script>
        var map = L.map("mapid").setView
            ([28.612894, 77.229446], 13); L.tileLayer
                ("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
                    attribution: "&copy; OpenStreetMap contributors",
                }).addTo(map);
        L.marker([28.612894, 77.229446])
            .addTo(map)
            .bindPopup("India Gate, New Delhi")
            .openPopup();
    </script>
</body>

</html>
```

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Output:</h4>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ 02. map image ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center" width="100%">
  <img src="./images/image-map-02.png"
  title="Map image."
  alt="Map image"
  style="border: 2px solid #000000; width:35%;" />
</p>
<!-- image-map02.jpg -->

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="04">04. </h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->


