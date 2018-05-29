---
title: "For Loops"
teaching: 10
exercises: 30
questions:
- "How can I make a program do something repeatedly?"
objectives:
- "Explain what for loops are normally used for."
- "Trace the execution of a simple (unnested) loop and correctly state the values of variables in each iteration."
- "Write for loops that use the Accumulator pattern to aggregate values."
keypoints:
- "A *for loop* executes commands once for each value in a collection."
- "The first line of the `for` loop must end with a colon, and the body must be indented."
- "A `for` loop is made up of a collection, a loop variable, and a body."
- "Loop variables can be called anything (but it is strongly advised to have a meaningful name to the looping variable)."
- "The body of a loop can contain many statements."
- "Use `range` to iterate over a sequence of numbers."
- "The Accumulator pattern turns many values into one."
---
> ## For loop structure:
> Label the parts (variable, collection, body) of this for loop: 
> ~~~ 
> for i in [2, 3, 5]:
>    print(i)
> ~~~
> {: .python}
{: .challenge}

> ## Variable names:
> Will this work?
> ~~~
> for kitten in [2, 3, 5]:
>    print(kitten)
> ~~~
> {: .python}
{: .challenge}

> ## Multiple expressions:
> ~~~
> primes = [2, 3, 5]
> ~~~
> {: .python}
> Write a for loop iterates over primes to produce:
> ~~~
> 2 4 8
> 3 9 27
> 5 25 125
> ~~~
> {: .output}
> 
{: .challenge}

> ## Accumulator patterns
> 
> *   A common pattern in programs is to:
>     1.  Initialize an *accumulator* variable to zero, the empty string, or the empty list.
>     2.  Update the variable with values from a collection using loop.
> 
> ~~~
> # Sum the first 10 integers.
> total = 0
> for number in range(10):
>    total = total + (number + 1)
> print(total)
> ~~~
> {: .python}
> Output:
> ~~~
> 55
> ~~~
> {: .output}
> Write out a table of execution line number and the value of `total` at each step for this program
{: .challenge}

> ## Practice Accumulating
>
> Fill in the blanks in each of the programs below
> to produce the indicated result.
>
> ~~~
> # Total length of the strings in the list: ["red", "green", "blue"] => 12
> total = 0
> for word in ["red", "green", "blue"]:
>     ____ = ____ + len(word)
> print(total)
> ~~~
> {: .python}
>
> ~~~
> # List of word lengths: ["red", "green", "blue"] => [3, 5, 4]
> lengths = ____
> for word in ["red", "green", "blue"]:
>     lengths.____(____)
> print(lengths)
> ~~~
> {: .python}
>
> ~~~
> # Concatenate all words: ["red", "green", "blue"] => "redgreenblue"
> words = ["red", "green", "blue"]
> result = ____
> for ____ in ____:
>     ____
> print(result)
> ~~~~
> {: .python}
>
> ~~~
> # Create acronym: ["red", "green", "blue"] => "RGB"
> # write the whole thing
> ~~~
> {: .python}
{: .challenge}


> ## Accumulator challenge 
> Use an accumulator pattern and a for loop to make a list of the first 10 fibonacci numbers.
>
> Hint: you will need to initialise two different kinds of variables before your for loop.
{: .challenge}

> ## Range
> ~~~
> my_collection = range(100)
> ~~~
> {: .python}
> 1. What is the type of `my_collection`?
> 2. Write a for loop that outputs the sum of all numbers 0 to 99.
> 3. Convert my_collection into a list.
> 4. Try the following:
>
> ~~~
> big_number = 100000000
> for i in range(big_number):
>     pass
> for i in list(range(big_number):
>     pass
> ~~~
> {: .python}
{: .challenge}

> ## Reversing a String
>
> Fill in the blanks in the program below so that it prints "nit"
> (the reverse of the original character string "tin").
>
> ~~~
> original = "tin"
> result = ____
> for char in original:
>     result = ____
> print(result)
> ~~~
> {: .python}
{: .challenge}

