---
title: "Libraries"
teaching: 5
exercises: 5
questions:
- "How can I use software that other people have written?"
- "How can I find out what that software does?"
objectives:
- "Explain what software libraries are and why programmers create and use them."
- "Write programs that import and use libraries from Python's standard library."
- "Find and read documentation for standard libraries interactively (in the interpreter) and online."
keypoints:
- "Most of the power of a programming language is in its libraries."
- "A program must import a library in order to use it."
- "Use `help` to find out more about a library's contents."
- "Import specific items from a library to shorten programs."
- "Create an alias for a library when importing it to shorten programs."
---


> ## Importing a library
> Without typing any numbers, get python to output:
> 
> ~~~
> pi is 3.141592653589793
> ~~~
> {: .output}
{: .challenge}

> ## Import options
>
> There are many ways to import a library or its functions. How 
> would you import so as to be able to call:
> ~~~
> my_rand = choice(['a','B', 2])
> my_rand = random.choice(['a','B', 2])
> my_rand = rd.choice(['a','B', 2])
> ~~~
> {: .python}
{: .challenge}

> ## No inheritance
>
> Again, without typing numbers, get python to output the cosine of pi.
>
{: .challenge}

> ## Help
> In Jupyter, works just like help for a function. Try:
> 
> ~~~
> help(math)
> ~~~
> {: .python}
 {: .challenge}

> ## Function import
> What are the benefits / disadvantages of importing like this:
> ~~~
> from math import cos, pi
> ~~~
> {: .python}
{: .challenge}

> ## When Is Help Available?
>
> When a colleague of yours types `help(math)`,
> Python reports an error:
>
> ~~~
> NameError: name 'math' is not defined
> ~~~
> {: .error}
>
> What has your colleague forgotten to do?
{: .challenge}

