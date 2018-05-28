---
title: "Conditionals"
teaching: 5
exercises: 20
questions:
- "How can programs do different things for different data?"
objectives:
- "Correctly write programs that use if and else statements and simple Boolean expressions (without logical operators)."
- "Trace the execution of unnested conditionals and conditionals inside loops."
keypoints:
- "Use `if` statements to control whether or not a block of code is executed."
- "Conditionals are often used inside loops."
- "Use `else` to execute a block of code when an `if` condition is *not* true."
- "Use `elif` to specify additional tests."
- "Conditions are tested once, in order."
- "Create a table showing updates to variables' values to trace the execution of a program."
---

> ## `if` statements within `for` loops 
> ~~~
> masses = [3.54, 2.07, 9.22, 1.86, 1.71]
> ~~~
> {: .python}
> Write some code that prints a value in `masses` if it is greater than 3:
> ~~~
> 3.54 is large
> 9.22 is large
> ~~~
> {: .output}
{: .challenge}

> ## Consequences ...
> modify your code above to produce the following: 
> ~~~
> 3.54 is large
> 2.07 is small
> 9.22 is large
> 1.86 is small
> 1.71 is small
> ~~~
> {: .output}
{: .challenge}
> ## Choices, choices ...
> 
> Modify your code again to produce the following:
> ~~~
> 3.54 is large
> 2.07 is small
> 9.22 is HUGE
> 1.86 is small
> 1.71 is small
> ~~~
> {: .output}
{: .challenge}

> ## Evaluation order
> 
> What is the outcome of this code?
>
> ~~~
> grade = 85
> if grade >= 70:
>     print('grade is C')
> elif grade >= 80:
>     print('grade is B')
> elif grade >= 90:
>     print('grade is A')
> ~~~
> {: .python}
> Modify the code above to produce the correct grade.
{: .challenge}

> ## Evolving variables
> Consider the following code:
> ~~~
> velocity = 10.0
> for i in range(5): # execute the loop 5 times
>     print(i, ':', velocity)
>     if velocity > 20.0:
>         print('moving too fast')
>         velocity = velocity - 5.0
>     else:
>         print('moving too slow')
>         velocity = velocity + 10.0
> print('final velocity:', velocity)
> ~~~
> {: .python}
> Create a table tracing the execution of this code. 
{: .challenge}

> ## Trimming Values
>
> Fill in the blanks so that this program creates a new list
> containing zeroes where the original list's values were negative
> and ones where the origina list's values were positive.
>
> ~~~
> original = [-1.5, 0.2, 0.4, 0.0, -1.3, 0.4]
> result = ____
> for value in original:
>     if ____:
>         result.append(0)
>     else:
>         ____
> print(result)
> ~~~
> {: .source}
>
> ~~~
> [0, 1, 1, 1, 0, 1]
> ~~~
> {: .output}
{: .challenge}

> ## Processing Small Files
>
> Modify this program so that it only prints the names of files with fewer than 50 records.
>
> ~~~
> import glob
> import pandas
> for filename in glob.glob('data/*.csv'):
>     contents = pandas.read_csv(filename)
>     ____:
>         print(filename, len(contents))
> ~~~
> {: .source}
{: .challenge}

> ## Initializing
>
> Modify this program so that it finds the largest and smallest values in the list
> no matter what the range of values originally is.
>
> ~~~
> values = [...some test data...]
> smallest, largest = None, None
> for v in values:
>     if ____:
>         smallest, largest = v, v
>     ____:
>         smallest = min(____, v)
>         largest = max(____, v)
> print(smallest, largest)
> ~~~
> {: .source}
>
{: .challenge}
