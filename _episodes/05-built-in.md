---
title: "Built-in Functions and Help"
teaching: 5
exercises: 10
questions:
- "How can I use built-in functions?"
- "How can I find out what they do?"
objectives:
- "Explain the purpose of functions."
- "Correctly call built-in Python functions."
- "Correctly nest calls to built-in functions."
- "Use help to display documentation for built-in functions."
keypoints:
- "A function may take zero or more arguments."
- "Commonly-used built-in functions include `max`, `min`, and `round`."
- "Functions may only work for certain (combinations of) arguments."
- "Functions may have default values for some arguments."
- "Use the built-in function `help` to get help for a function."
- "Every function returns something."
---

> ## Function anatomy
>
> Name the parts of this statement:
>
> ~~~
> x = max(1, 2, 3)
> ~~~
> {: .python}
> Is this a valid function call?
> ~~~
> print()
> ~~~
> {: .python}
{: .challenge}

> ## Arguments
>
> Try out the following:
>
> ~~~
> max('a','A','0')
> ~~~
> {: .python}
> ~~~
> max('a','A', 0)
> ~~~
> {: .python}
> ~~~
> max()
> ~~~
> {: .python}
{: .challenge}

> ## Defaults
> What is the result?
> ~~~
> pi = 3.712
> round(pi)
> ~~~
> {: .python}
> Use `round` to calculate `pi` to one decimal place.
> Hint: try
> ~~~
> round?
> ~~~
> {: .python}
{: .challenge}

> ## Return values
>
> Predict the outcome of the following two examples:
> ~~~
> largest = max(1,5,3,8,20,3)
> print('The largest value is:', largest')
> ~~~
> {: .python}
> ~~~
> result = print('example')
> print('result of print is', result)
> ~~~
> {: .python}
{: .challenge}

> ## Order of operations
>
> 1. Explain in simple terms the order of operations in the following program:
>    when does the addition happen, when does the subtraction happen,
>    when is each function called, etc.
> 2. What is the final value of `radiance`?
>
> ~~~
> radiance = 1.0
> radiance = max(2.1, 2.0 + min(radiance, 1.1 * radiance - 0.5))
> ~~~
> {: .source}
>
> Predict the outcome of both `or` statements below:
> ~~~
> first_value = 1
> first_value or second_value
> second_value or first_value
> ~~~
{: .challenge}
{: .challenge}

> ## Spot the Difference
>
> 1. Predict what each of the `print` statements in the program below will print.
> 2. Does `max(len(rich), impoverished)` run or produce an error message?
>    If it runs, does its result make any sense?
>
> ~~~
> rich = "gold"
> impoverished = "tin"
> print(max(rich, impoverished))
> print(max(len(rich), len(impoverished)))
> ~~~
> {: .source}
{: .challenge}

> ## Why Not?
>
> Why don't `max` and `min` return `None` when they are given no arguments?
{: .challenge}
