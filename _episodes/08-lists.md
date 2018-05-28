---
title: "Lists, Strings, and Indexing"
teaching: 10
exercises: 10
questions:
- "How can I store multiple values?"
objectives:
- "Explain why programs need collections of values."
- "Write programs that create flat lists, index them, slice them, and modify them through assignment and method calls."
keypoints:
- "A list stores many values in a single structure."
- "Use an item's index to fetch it from a list."
- "Lists' values can be replaced by assigning to them."
- "Appending items to a list lengthens it."
- "Use `del` to remove items from a list entirely."
- "The empty list contains no values."
- "Lists may contain values of different types."
- "Character strings can be indexed like lists."
- "Character strings are immutable."
- "Indexing beyond the end of the collection is an error."
---

> ## Slicing
>
> What does the following program print? Try
> drawing the list to work it out, then test your
> working using the code.
>
> ~~~
> element = 'carbon'
> print('element[1:3] is:', element[1:3])
> ~~~
> {: .python}
>
> 1.  What does `thing[low:high]` do?
> 2.  What does `thing[low:]` (without a value after the colon) do?
> 3.  What does `thing[:high]` (without a value before the colon) do?
> 4.  What does `thing[:]` (just a colon) do?
{: .challenge}

> ## Fill in the Blanks
>
> Fill in the blanks so that the program below produces the output shown.
>
> ~~~
> values = ____
> values.____(1)
> values.____(3)
> values.____(5)
> print('first time:', values)
> ____ values[____]
> print('second time:', values)
> ~~~
> {: .python}
> Output:
> ~~~
> first time: [1, 3, 5]
> second time: [3, 5]
> ~~~
> {: .output}
{: .challenge}

> ## How Large is a Slice?
>
> If 'low' and 'high' are both non-negative integers,
> how long is the list `values[low:high]`?
{: .challenge}

> ## From Strings to Lists and Back
>
> Fill in the blanks:
>
> ~~~
> my_str = 'tin'
> my_list = ['g', 'o', 'l', 'd']
> print('string to list:', ____(____))
> print('list to string:', ____.____(____))
> ~~~
> {: .python}
> Output:
> ~~~
> ['t', 'i', 'n']
> 'gold'
> ~~~
> {: .output}
>
{: .challenge}

> ## Working With the End
>
> What does the following program print?
>
> ~~~
> element = 'helium'
> print(element[-1])
> ~~~
> {: .python}
>
> 1.  How does Python interpret a negative index?
> 2.  If a list or string has N elements,
>     what is the most negative index that can safely be used with it,
>     and what location does that index represent?
> 3.  If `values` is a list, what does `del values[-1]` do?
> 4.  How can you display all elements but the last one without changing `values`?
>     (Hint: you will need to combine slicing and negative indexing.)
{: .challenge}

> ## Stepping Through a List
>
> What does the following program print?
>
> ~~~
> element = 'fluorine'
> print(element[::2])
> print(element[::-1])
> ~~~
> {: .python}
>
> 1.  If we write a slice as `low:high:stride`, what does `stride` do?
> 2.  What expression would select all of the even-numbered items from a collection?
{: .challenge}

> ## Bounds
>
> What does the following program print?
>
> ~~~
> element = 'lithium'
> print(element[0:20])
> print(element[-1:3])
> print(element[20])
> ~~~
> {: .python}
{: .challenge}

> ## Indexes
> ~~~
> str_element = 'heliam'
> list_element = ['h', 'a', 'l', 'i', 'u', 'm']
> ~~~
> {: .python}
> Which of the following two expressions will execute?
> ~~~
> str_element[4] = 'u'
> list_element[1] = 'e'
> ~~~
> {: .python}
{: .challenge}
