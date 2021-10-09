# LaTeX Copypasta

I'm slowly amassing lists of course-related LaTeX macro definitions that make it faster to type notes and assignments without worrying about typesetting. This repo contains copypastas for the following University of Waterloo courses:

- MATH 235 - Linear Algebra 2 (online, fall 2020)
- CS 341 - Algorithms (online, fall 2020)
- CS 348 - Introduction to Database Management (online, spring 2021)
- CS 370 - Numerical Computation (online, fall 2020)
- CS 486 - Introduction to Artificial Intelligence (online, spring 2021)
- STAT 330 - Mathematical Statistics (online, spring 2021)
- STAT 333 - Applied Probability (online, spring 2021)

## Example

```
% without macros
\left\lbrace \left\lfloor e^x \right\rfloor \ \middle|\  x \in \Z \right\rbrace

% with macros
\set{ \floor{e^x} \where x \in \Z }
```

## Getting Started

First, clone this repository (of course).

### LaTeX

To include a copypasta in your LaTeX file, simply add `\input{path-to-copypasta.tex}` above wherever you want to use the macros.

### Typora

I write my notes and assignments in Markdown using Typora. Typora has the benefit over pure LaTeX of being mostly WYSIWYG while still supporting math and code blocks. Typora also happens to support macro definitions via `\newcommand`. Any commands defined at the top of the document can be reused throughout.

To include a copypasta in Typora, simply copy it into a multiline equation block (surrounded by `$$`) at the top of the document.

#### Inline LaTeX in Typora, how?

`File` > `Preferences` > `Markdown` > `Syntax Support` > `Inline Math` = `On`

#### All the equations are broken?

`Edit` > `Math Tools` > `Refresh All Math Expressions`

#### All the equations are still broken?

Close the document (after saving) and reopen it.
