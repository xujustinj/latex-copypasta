# LaTeX Copypasta

I'm slowly amassing lists of LaTeX macro definitions that make it faster to type assignments without worrying about typesetting.

## In This Repo

`pasta.*.sty` files are copypastas, named that way to avoid naming collisions with actual packages. `course.*.sty` files then collect multiple copypastas into a single `usepackage`-able file for the following University of Waterloo courses:

- **CS 341: Algorithms** (fall 2020)
- **CS 348: Introduction to Database Management** (spring 2021)
- **CS 370: Numerical Computation** (fall 2020)
- **CS 486: Introduction to Artificial Intelligence** (spring 2021)
- **MATH 235: Linear Algebra 2** (fall 2020)
- **STAT 330: Mathematical Statistics** (spring 2021)
- **STAT 331 / SYDE 334: Applied Linear Models** (winter 2022)
- **STAT 333 Applied Probability** (spring 2021)

No guarantees on completeness here. Some courses (especially those I didn't take notes for in LaTeX) are missing commands for things that didn't come up in assignments.

## Usage

### LaTeX

Add `\usepackage{path/to/sty_file_without_extension}` to the top of your `.tex` or `.sty` file.

> It is best to put a copy of the copypasta files you need in the same directory as wherever you are including it, as `usepackage` with paths is not standard.

### R Markdown

Add the following to the YAML preamble:

```yaml
header-includes:
  - \usepackage{path/to/sty_file_without_extension}
```

> The same advice about directories from [Usage - LaTeX](#latex) applies here.

### Typora

[Typora](https://typora.io/) supports macro definitions via `\newcommand`. Any commands defined at the top of the document can be reused throughout. To use copypastas in Typora:

1. **(optional, once per Typora installation)** To use LaTeX inline (e.g. `$ \pr{ x + y }^3 $`), enable inline LaTeX math in Typora by setting `File` > `Preferences` > `Markdown` > `Syntax Support` > `Inline Math` = `On`.
1. Copy one or more copypastas into a single multiline equation block (surrounded by `$$`) at the top of the document.
1. Delete any `\usepackage{...}` lines you see.

If your equations suddenly cannot find the copypasta command definitions, try `Edit` > `Math Tools` > `Refresh All Math Expressions`. If they are still broken, close the document (after saving) and reopen it.

## Example

```
% without copypasta
\left\lbrace \left\lfloor e^x \right\rfloor \ \middle|\  x \in \Z \right\rbrace

% with copypasta
\set{ \floor{e^x} \where x \in \Z }
```

## Documentation

Sorry, you'll have to dig through the `.sty` files yourself.
