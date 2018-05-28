---
title: "Jupyter Gurus"
teaching: 5
exercises: 10
questions:
- "Review of Jupyter commands"
objectives:
- "Launch the Jupyter Notebook, create new notebooks, and exit the Notebook."
- "Create Markdown cells in a notebook."
- "Create and run Python cells in a notebook."
keypoints:
- "Use the Jupyter Notebook for editing and running Python."
- "The Notebook has Control and Edit modes."
- "Use the keyboard and mouse to select and edit cells."
---

> ## Jupyter
> Open and save a new Jupyter Notebook for today's work.
>
> Perform a mathematical calculation in the first cell.
>
> Where is your new notebook stored?
{: .challenge}

> ## How are Jupyter Notebooks and Vim similar?
>
> Press "esc" and "return" alternately. What does this do?
>
> Press "esc", "return", "h".
>
> Use shortcuts to make a new cell above the calculation cell, and
> write a title for your notebook in markdown.
{: .challenge}

> ## The keyboard
> 
> Without using the mouse, edit your code cell to multiply the
> calculation by two, and rerun it
{: .challenge}

> ## Creating lists in markdown
>
> Create a nested list in a Markdown cell in a notebook that looks like this:
>
> 1.  Get funding.
> 2.  Do work.
>     *   Design experiment.
>     *   Collect data.
>     *   Analyze.
> 3.  Write up.
> 4.  Publish.
{: .challenge}

> ## Code cell output
>
> What is displayed when a Python cell in a notebook
> that contains several calculations is executed?
> For example, what happens when this cell is executed?
>
> ~~~
> 7 * 3
> 2 + 1
> ~~~
> {: .source}
{: .challenge}

> ## Code as markdown
>
> What happens if you write some Python in a code cell
> and then you switch it to a Markdown cell?
> For example,
> put the following in a code cell:
>
> ~~~
> x = 6 * 7 + 12
> print(x)
> ~~~
> {: .python}
>
> And then run it with shift+return to be sure that it works as a code cell.
> Now go back to the cell and use escape+M to switch the cell to Markdown
> and "run" it with shift+return.
>
> What happened and how might this be useful?
{: .challenge}

> ## Mathematics
>
> Standard Markdown (such as we're using for these notes) won't render equations,
> but the Notebook will.
> Create a new Markdown cell
> and enter the following:
>
> ~~~
> $\Sigma_{i=1}^{N} 2^{-i} \approx 1$
> ~~~
> {: .source}
>
> What does it display?
> What do you think the underscore `_`, circumflex `^`, and dollar sign `$` do?
{: .challenge}

[markdown]: https://en.wikipedia.org/wiki/Markdown
