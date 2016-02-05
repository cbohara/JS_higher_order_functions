## Exercise: Intro to Higher Order Functions

## Overview:

	Today you were introduced to the magical world of Higher Order Functions. Being able to create and conceptualize higher order functions so easily is why JavaScript is one of the most popular languages in the programming world. 

	As your lecturer mentioned, HRF's are the key to building more declaritive and expressive code. Code that's more legible, and translatable allows us more time to do what we want to be doing: building.

	Take, doMathSoIDontHaveTo examples from the slides:

```
		var increment = function(n){
  			return n + 1;
		};

		var square = function(n){
  			return n*n;
		};

		var doMath = function(n, func){
			// returns the callback evaluated callback to the user
  			return func(n);
		};

		var twentyFive = doMath(5, square);

		var five = doMath(4, increment);

```

	First, instead of having to parse through parse through mathematical algorithms, we've translated our action to two functions: increment, and square. 

	Secondly, we took the extra step and abstracted out even further by building a function that evaluates our two functions even further. Now, whenever someone reads through our code they'll know that we're doing some math on that line, with that function. Now, whenever I need to do some math, I don't have to think about pseudocoding it out; I have an expressive action I can take to make it happen.

	The philosophy of Functional Programming is powerful. It saves time, effort (programmers are lazy, remember?), and allows us to build some really cool stuff. Higher Order Functions are a key part of that, and this lesson will help you get down the basic.


	###Remember your Key Takeaways:

		A higher order function is a function that takes a function as input and/or returns a function as output:

```
					// higher order function
					var doMath = function(n, func){ // takes a callback as a parameter
						// returns the callback evaluated callback to the user
  						return func(n);
					};

```

		"Callback" is a term used for any function that is passed as an argument to a function they can be named or anonymous arguments for callbacks can be passed as arguments to the higher order function:

``` 
				//callback, when passed into the doMath function
				var increment = function(n){
  					return n + 1;
				};

				//callback, when passed into the doMath function
				var square = function(n){
  					return n*n;
				};

				var doMath = function(n, func){
				
  					return func(n);
				};
				// increment callback
				var five = doMath(4, increment)

				// callback as anonymous function
				var twentyFive = doMath(5, function(n){ n*n })



```

## What you should be comfortable with:

	- Syntax for accessing and creating objects, arrays, and functions
	- Scope and how variable access works in JavaScript
	- Algorithmic approach and programming problems step by step
	- Pseudocoding


## Learning Goals:

	- Strengthen your understanding of higher order functions, callbacks and anonymous functions.
	- Practicing debugging skills without the tests
	- Further transition you toward mastering functional programming.

