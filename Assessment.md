# Return and print are different things

Many people mistakenly believe that the code will print x = hi, but it does not. foo() prints "hi" when it runs, but the return value of the function is undefined by default, which is why x gets assigned undefined.

# Multiple Different Return Statements Inside a Single Function

Many people assume that the final print statement will execute multiple times, but it only prints once. The return statements inside the function dictate the flow. The function foo("blue") will return 1, and foo("red") will return 2. However, only the final value of x is printed.

# Return Statements Inside For Loops

In this example, the return statement inside the for loop will cause the loop to terminate after the first iteration. The function immediately returns the value of i when it hits the return statement, so x will only be assigned the first value of i.

# Function Arguments/Parameters

The function foo uses the rest parameter ...args, which collects all arguments passed to the function into an array. Even though no arguments are passed when calling foo(), the function still returns an empty array ([]), not null or undefined.

# Hoisting

JavaScript has a behavior called "hoisting," where function declarations are hoisted to the top of their scope. This allows you to call foo() before its declaration in the code, and it will still work without raising an error.
