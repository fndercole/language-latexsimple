# language-latexsimple

This is an alternative package for Atom editor that support LaTeX, TeX and BibTeX grammar syntax.

## Features
### Comments
  - In-line comments, `% commented text`.
  - Multi-line comments blocks, `\begin{comment} ... \end{comment}`.
  - TODO tags in comments importing `source.todo`.

### Verbatim
  - In-line verbatim `\verb|<verbatim text>|`.
  - Verbatim environment blocks `\begin{verbatim} ... \end{verbatim}`.
  - Support other source code highlight, beginning with `% language:` and ending with `% end`. Currently, support this scopes:
    - R: `source.r`
    - STATA: `source.stata`
    - Shell: `source.shell`

    I plan to support any scope, but I need more knowledge about coffeeScript to achieve that.

### Commands
  - Generic commands of the form `\command`.
  - TeX commands of the form `\foo@bar`.
  - Document class declaration such as
    - `documentclass[<optional args>]{<class>}`
  - Including declarations such as
    - `\usepackage[<optional args>]{<packages>}`
    - `\input[<optional args>]{<files>}`
    - `\include[<optional args>]{<files>}`
    - `\includegraphics[<optional args>]{<file>}`
    - `\bibliography[<optional args>]{<file>}`
    - `\nobibliography[<optional args>]{<file>}`
  - Headings declarations such as
    - `\title[<optional args>]{<heading>}`
    - `\part[<optional args>]{<heading>}`
    - `\chapter[<optional args>]{<heading>}`
    - `\section[<optional args>]{<heading>}`
    - `\subsection[<optional args>]{<heading>}`
    - `\paragraph[<optional args>]{<heading>}`

### Environments
  - Generics environment blocks `\begin{<environment>} ... \end{<environment>}`

### Mathematics
  - In-line math `$ ... $`
  - Display math blocks `\[ ... \]`
  - Math environments beginning with `\begin{equation}` or `\begin{align}`.
  - Match any of this delimiters: `\left\{`, `\left[`, `\left(`, `\left.` with any of: `\right\}`, `\right]`, `\right)`, `\right.`.

### Punctuation
  - Highlights `&`, `_`, `^`, `\\`, `.`, `-`.

### Groups
  - Nested groups using `{` and `}`. Non matched `}` is not highlighted.
  - Match `(`, `)`.
  - Match `[`, `]`. Inside brackets groups highlights keyword `foo = bar`.

### BibTeX
  - Entry environment `@entry{...}`.
  - Citation key, `key1999,`
  - tag `foo = ... ,`

### Files
  - `text.tex.latex` is active on `tex`, `sty` and `cls` files.
  - `text.tex.bibtex` is active on `bib` files.


## TODO's
  - Add support for other grammar into verbatim environments.
  - Improve Support for TeX files like `sty`, `cls` and `ltx`.
  - Add more escaped symbols.
  - Add special support for subsubsectioning.
  - Add support for special pstricks commands.

## Related projects

  - [Varone Dark Syntax](https://github.com/fndercole/varone-dark-syntax), provide colours name declared in this grammar.
  - [linter-spell-latexsimple](https://github.com/fndercole/linter-spell-latexsimple), is a compatible provider for [linter-spell](https://github.com/yitzchak/linter-spell).

## Warnings

You must disable `language-latex` or `language-tex` before enable this.

The older package `language-latex` has some issues, so I write from scratch a new package. This is not a fork, so there is no compatibility warranty.

This software is in alpha stage of development. Please, add an issue for request a feature.
