---
title: "Data Types and Type Conversion"
teaching: 5
exercises: 5
questions:
- "What kinds of data do programs store?"
- "How can I convert one type to another?"
objectives:
- "Explain key differences between integers and floating point numbers."
- "Explain key differences between numbers and character strings."
- "Use built-in functions to convert between integers, floating point numbers, and strings."
keypoints:
- "Every value has a type."
- "Use the built-in function `type` to find the type of a value."
- "Types control what operations can be done on values."
- "Strings can be added and multiplied."
- "Strings have a length (but numbers don't)."
- "Must convert numbers to strings or vice versa when operating on them."
- "Can mix integers and floats freely in operations."
---


~~~
print(type(42))
~~~
{: .python}
~~~
print(type(life))
~~~
{: .python}

~~~
print(type(author))
~~~
{: .python}

> ## Types and operations
> 
> Try:
> ~~~
> length(author)
> length(life)
> ~~~
> {: .python}
{: .challenge}

> ## Attributes
>
> Try:
> ~~~
> dir(life)
> ~~~
> {: .python}
>
> Try out life's bit_length attribute. 
> How can you get help with an object's attributes in Jupyter?
{: .challenge}

> ## Type conversion
> predict the outcome of these statements:
> ~~~
> print(1, 'A')
> print(1 + 'A')
> ~~~
> {: .python}
> Modify the second statement so that it works
>
> What about:
> ~~~
> print(1 + '2')
> ~~~
> {: .python}
{: .challenge}

> ## Choose a Type
>
> What type of value (integer, floating point number, or character string)
> would you use to represent each of the following?
>
> 1. Number of days since the start of the year.
> 2. Time elapsed since the start of the year.
> 3. Serial number of a piece of lab equipment.
> 4. A lab specimen's age.
> 5. Current population of a city.
> 6. Average population of a city over time.
{: .challenge}

> ## Division Types
>
> What is the difference between the `//` operator and 
> the '%' operator? Let's find out:
>
> ~~~
> 5//3
> 5%3
> ~~~
> {: .python}
>
> Coding challenge: If `num_subjects` is the number of subjects taking part in a study,
> and `num_per_survey` is the number that can take part in a single survey,
> write an expression that calculates the number of surveys needed
> to reach everyone once.
{: .challenge}

> ## Strings to Numbers
>
> What is the problem with this statement?
>
> ~~~
> print("fractional string to int:", int("3.4"))
> ~~~
> {: .python}
{: .challenge}

> ## Arithmetic with Different Types
>
> Which of the following will print 2.0?
> Note: there may be more than one right answer.
>
> ~~~
> first = 1.0
> second = "1"
> third = "1.1"
> ~~~
> {: .python}
>
> 1. `first + float(second)`
> 2. `float(second) + float(third)`
> 3. `first + int(third)`
> 4. `first + int(float(third))`
> 5. `int(first) + int(float(third))`
> 6. `2.0 * second`
{: .challenge}
