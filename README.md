# language-latexsimple

This is an alternative package for Atom editor that support LaTeX grammar syntax.

I use this with [Varone Dark Syntax](https://github.com/fndercole/varone-dark-syntax), which support specific selectors declared in latex.cson.

## Features
  - Identify inline comments, `% comment text`.
  - Identify multiline comments blocks, `\begin{comment} ... \end{comment}`.
  - Identify generic command of the form `\command`.
  - Identify special declaration such as
    - `documentclass[<optional args>]{<class>}`
  - Identify include declarations such as
    - `\usepackage[<optional args>]{<packages>}`
    - `\input[<optional args>]{<files>}`
    - `\include[<optional args>]{<files>}`
    - `\includegraphics[<optional args>]{<file>}`
    - `\bibliography[<optional args>]{<file>}`
    - `\nobibliography[<optional args>]{<file>}`
  - Identify sectioning declarations such as
    - `\title[<optional args>]{<heading>}`
    - `\part[<optional args>]{<heading>}`
    - `\chapter[<optional args>]{<heading>}`
    - `\section[<optional args>]{<heading>}`
    - `\subsection[<optional args>]{<heading>}`
    - `\paragraph[<optional args>]{<heading>}`
  - Identify inline math `$ ... $`
  - Identify display math blocks `\[ ... \]`
  - Identify generic environment blocks `\begin{<environment>} ... \end{<environment>}`
  - Identify `\verb|<verbatim text>|`.
  - Identify verbatim environment blocks `\begin{verbatim} ... \end{verbatim}`.
  - Identify `[`, `]`, `{` and `}`
  - Support `*.tex` files
  - Support `TODO` tags (`text.todo` scope) in inline comments. `% TODO: foo bar`
  - Allow embedded R grammar throught special comments:

    ```
    % language: R

      \begin{verbatim}

        < some R code >

      \end{verbatim}

    % end
    ```

## TODO's
  - [ ] Add support for other grammar into verbatim environments.
  - [ ] Support for TeX files like `sty`, `cls` and `ltx`.
  - [ ] Add escaped symbols.
  - [ ] Add special support for subsubsectioning.
  - [ ] Add suport for special pstricks commands.
  - [ ] Add snippets.

## Warnings

You must disable `language-latex` or `language-tex` before enable this.

If you want spell checking support, install `linter-spell-latexsimple`.

This software is in alpha stage of development. Please, add an issue for request a feature.
