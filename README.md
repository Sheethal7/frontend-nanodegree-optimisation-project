# Website Performance Optimization portfolio project

## Getting started
* Clone or fork the repository
* Open the html files and run through any browser to view the page

### Part 1: Optimize PageSpeed Insights score for index.html
* Open index.html in a browser of your choice
* Run the file through PageSpeed Insights to view score

#### Optimisations:
##### index.html:
* CSS loading was done asynchronously using requestAnimationFrame
* Critical css files were inlined
* media query for print was included in the link tag as media=print
* Java Script files is now loaded in the head tag
* Images were optimised using an online tool https://kraken.io/

### Part 2: Optimize Frames per Second in pizza.html
* Open pizza.html in a browser of your choice
* Open Timeline in Developer tools to view whether the page runs at 60fps

#### Optimisations:
##### views/pizza.html:
* Style tags were removed as much as possible
* Bootstrap Classes were assigned instead of width in style tags
* Images were optimised using an online tool https://kraken.io/

#####  views/js/main.js:
* Strict mode was enabled by including 'use strict';
* document.querySelector() was replaced by document.getElementById() Web API
* array length is saved in a local variable outside the conditional statement
* document.querySelectorAll() was replaced by document.getElementsByClassName() Web API
* document.getElementsByClassName('randomPizzaContainer') is stored in a local varioable outside the loop
* document.body.scrollTop / 1250; is saved in a local variable outside the loop
* Number of background pizzas were reduced to 24
* The elem variable (var elem;) is declared in the initialisation of the for-loop

##### views/css/style.css:
* hardware accelerated CSS was included to increase performance
* vendor prefixes were added# frontend-nanodegree-optimisation-project
