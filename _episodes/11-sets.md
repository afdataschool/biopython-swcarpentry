---
title: "Sets"
teaching: 5
exercises: 25
questions:
- "What is a set, and how do I use it?"
objectives:
- "Explain how sets work."
- "Learn about set operations"
keypoints:
- "A set stores unsorted unique values."
- "Sets may contain values of different types."
---
> ## Sets are containers of unsorted unique values
>
> ~~~
> beatles = set(['John', 'Paul', 'George', 'Ringo'])
> print('Beatles:', beatles)
> print('length:', len(beatles))
> beatles.add('Ringo')
> ~~~
> {: .python}
> Predict what the output of the following two expressions:
> ~~~
> print('Beatles:', beatles)
> print('length:', len(beatles)
> ~~~
> {: .python}
{: .challenge}


> ## Checking membership
> Write a single line of code that produces the following output:
> ~~~
> Ringo is one of the Beatles: True
> Keith is one of the Beatles: False
> ~~~
> {: .output}
{: .challenge}

> ## Adding values
>
> Add in your favourite fifth Beatle to get this output:
> ~~~
> beatles is now: {'Stuart', 'John', 'Ringo', 'Paul', 'George'}
> ~~~
> {: .output}
> Did you all get the same output?
{: .challenge}

> ## Removing values
> Stuart's down on his luck, having passed away in 1962. Let's remove him again:
> ~~~
> beatles is now: {'John', 'Ringo', 'Paul', 'George'}
> ~~~
> {: .output}
> Are sets mutable or immutable? 
{: .challenge}

> ## Set operations
> 
> ~~~
> Beatles_official = set(['Ringo', 'Paul', 'George', 'John'])
> Beatles_alive = set(['Ringo', 'Paul, 'Pete'])
> ~~~
> {: .python}
> 1. On a piece of paper, use set diagrams to depict the 'unofficial' Beatle(s) 
> that are still alive.
> 2. Write some Python code that determines the existing unofficial Beatle. 
{: .challenge}


> ## Difference between two sets
> 
> Do these two expressions give the same result?
> ~~~
> Beatles_official.difference(Beatles_alive)
> Beatles_alive.difference(Beatles_official)
> ~~~
> {: .python}
{: .challenge}


> ## Order
>
> 1. Make a `set` containing the prime numbers between 0 and 20
> Make another `set` containing the even numbers between 0 and 20. 
> Use set operations to print out the prime numbers that are even.
> 
> 2. Now, print them out in a more 'orderly' fashion. HINT: what structure could you use to store an *indexed* collection? 
{: .challenge}

> ## Fill in the Blanks
>
> Fill in the blanks so that the program below produces the output shown.
>
> ~~~
> multiples_of_two = set([2, 4, 6, 8, 10])
> multiples_of_three = set([3, 6, 9])
> result1 = multiples_of_two._______(multiples_of_three)
> print('1', result1)
> result2 = multiples_of_____.______(multiples_of______)
> sorted_result2 = list(result2)
> sorted_result2.sort()
> print('2', sorted_result2)
> ~~~~
> {: .python}
>
> ~~~
> 1 {6}
> 2 [3, 9]
> ~~~
> {: .output}
{: .challenge}

> ## Set types
> Is this a valid set?
> ~~~
> my_collection=set([42, 'Galaxy', 3.71])
> ~~~
> {: .python}
{: .challenge}
