# language-latexsimple

This is an alternative package for Atom editor that support LaTeX grammar syntax.

## Features
  - Identify generic comand of the form `\commad`.
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
  - Identify `[`, `]`, `{` and `}`
  - Support `*.tex` files

## TODO's
  - [ ] Add support for other grammar into verbatim environments.
  - [ ] Add support for multiline comments.
  - [ ] Support for TeX files like `sty`, `cls` and `ltx`.
  - [ ] Add escaped symbols.
  - [ ] Add special support for subsubsectioning.
  - [ ] Add suport for special pstricks commands.

## Warnings

You must disable `language-latex` or `language-tex` before enable this.

This software is in alpha stage of development. Please, add an issue for request a feature.
