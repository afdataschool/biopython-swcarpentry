---
title: "Variables and Assignment"
teaching: 5
exercises: 10
questions:
- "How can I store data in programs?"
objectives:
- "Write programs that assign values to variables and perform calculations with those values."
- "Correctly trace value changes."
keypoints:
- "Use variables to store values."
- "Use `print` to display values."
- "Variables persist between cells."
- "Variables must be created before they are used."
- "Python is case-sensitive."
- "Use meaningful variable names."
- "Variables can be used in calculations."
- "Variable assignment creates a new variable."
- "Mutability matters!"
---

> ## Variable assignment
>
> What is the meaning of life?  (Hint: if you don't know google 'hitchiker meaning of life')
> 
> Store this in a variable called 'life'. 
>
> What is the 'type' of life? Get Python to print this for you.
{: .challenge}                                               

> ## Legal names
>
> Which of the following statements use legal Python variable names?
>
> ~~~
> 42Douglas_Adams = "The answer to the ultimate question of life, the universe and everything is 42."
> douglas = 'The answer to the ultimate question of life, the universe and everything is 42.'
> douglas_adams = "The answer to the ultimate question of life, the universe and everything is 42."
> douglas42 = "The answer to the ultimate question of life, the universe and everything is 42."
> Douglas = "The answer to the ultimate question of life, the universe and everything is 42."
> douglas-adams = 'The answer to the ultimate question of life, the universe and everything is 42.'
> _douglas_adams = "The answer to the ultimate question of life, the universe and everything is 42."
> ~~~
> {: .source}
{: .challenge}

> ## Printing
>
> Store 'Douglas Adams' in a variable called 'author'.
> Use a print statement and your two variables to display 
> 'Douglas Adams defined the meaning of life to be 42'.
{: .challenge}

> ## Persistence
>
> Go back to your orginal cell where you defined the meaning of life.
>
> Redefine the meaning of life to be anything you like.
>
> Rerun the cell with the previous print statement. Is this what you expect?
{: .challenge}

> ## Existence
>
> Try this code:
> ~~~
> print(Author)
> ~~~
> {: .source}
{: .challenge}

> ## Calculation
>
> What do these statements do?
>
> ~~~
> reincarnation = life * 2
> author * life
> life = life - 10
> author + life 
> ~~~
> {: .source}
{: .challenge}

> ## Swapping Values
>
> Draw a table showing the values of the variables in this program
> after each statement is executed.
> In simple terms, what do the last three lines of this program do?
>
> ~~~
> lowest = 1.0
> highest = 3.0
> temp = lowest
> lowest = highest
> highest = temp
> ~~~
> {: .source}
{: .challenge}

> ## Predicting Values
>
> What is the final value of `position` in the program below?
> (Try to predict the value without running the program,
> then check your prediction.)
>
> ~~~
> initial = "left"
> position = initial
> initial = "right"
> ~~~
> {: .source}
{: .challenge}

> ## Mutability
>
> Take a guess at the final value of both variables in each code block below. 
> Try out the code. Does it work as expected?
> ~~~
> num_str = '123456'
> rev_str = num_str
> num_str = num_str[::-1] 
> ~~~
> {: .source}
>
> (the [::-1] is code to reverse a string)
> ~~~
> num_list = [1,2,3,4,5,6]
> rev_list = num_list
> num_list.reverse() 
> rev_list.append(7)
> ~~~
> {: .source}
>
> Now type:
> ~~~
> num_list = [99,100]
> ~~~
> {: .source}
> What is the final value of num_list and rev_list?
{: .challenge}
> {: .source}
