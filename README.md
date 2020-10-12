# Typora LaTeX Copypasta

This term I switched to writing notes and assignments in Markdown (Typora). It has the benefit over pure LaTeX of being mostly WYSIWYG while still supporting math and code blocks. Another great thing about Typora is that it supports `\newcommand`. Any commands defined at the top of the document can be reused throughout.

I'm slowly amassing a huge list of course-related commands that make it faster to type notes and assignments without worrying about typesetting. [`copypasta.md`](https://raw.githubusercontent.com/xujustinj/Typora-LaTeX-Copypasta/main/copypasta.md) contains all the commands I have so far, wrapped in a single math block that can be nestled invisibly at the top of any document. Use it as a template for starting new note and assignment documents.

At the moment this library supports the following University of Waterloo courses:

* MATH 235 - Linear Algebra 2 (taken online, fall 2020)
* CS 341 - Algorithms (taken online, fall 2020)
* *coming soon*: CS 370 - Numerical Computation (taken online, fall 2020)

Eventually the library will probably get to the point where having multiple courses in the same copypasta will lead to conflicts... when that day comes I'll just split it into smaller copypastas.

# FAQ

#### Inline LaTeX in Typora, how?

`File` > `Preferences` > `Markdown` > `Syntax Support` > `Inline Math` = `On`

#### All the equations are broken?

`Edit` > `Math Tools` > `Refresh All Math Expressions`

#### All the equations are still broken?

Close the document (after saving) and reopen it.
