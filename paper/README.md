#Analysis of AI approaches

- **Venue:** [CCC'18](http://www.utb.edu.co/13ccc/articulos) 

## Description
Analyzing existing approaches to AI/ML what are they used for, what can't they do, when to use them.

The main file of the paper is _main.tex_ containing the structure definition and references to all input files. There is a file for each independent section of the paper.


## Structure 

* The generated pdf file of the paper should not be committed to the repository as it is continuously changing and can be generated locally. This avoid conflicts!!!
* preamble: contains all package and command definitions. Everything should be set by now, but if something needs defining this is the place to do it (look inside to see the structure)
* bibfiles
    * local.bib: contains all local bib references i.e., references used for this paper specifically. Most references should be added here
    * bib folder: this folder contains many references used for multiple purposes, in particular the _compsci.bib_ file contains many references on software engineering, programming languages, and adaptive systems. Check here if the reference exists before adding it to the _local.bib_ file
* Acronym.tex: contains all Acronyms used in the paper (look into the file for example of the definition). Acronyms are used with the \ac{ACRONYM} command (e.g., \ac{COP} for Context-Oriented Programming)
* Pointers to objects in the text (e.g., images, tables, code, sections, code-line, ....) are referenced using the fancyref package using the command \fref{} respectively starting with (img:, tab:, lst:, sec:, ln:, ....). The hyperref package is used to make sure references are clickable.
* Code is defined according to the specific language to display using the \begin{LANGUAGE} .. \end{LANGUAGE}. For example, for context traits one would use \begin{ctxtraits} .. \end{ctxtraits}. Inlined code is defined using the \scode{..} environment. If multiple languages are defined, the initial s is changed by the language name.

## Useful commands

* _\authorcomment[TYPE]{AUTHOR}{COMMENT}_ is used to leave annotation inlined with the text. Comments only appear in draft mode (the option in the documentclass in the _main.tex_ file) and are invisible otherwise. The comment type can be: comment, missing, idea, note, and author.
* _\ie \eg \cf_ (without curly braces) are used respectively for the abbreviations i.e., e.g., cf.
* listings are defined according to each specific language in the _preamble_ file and generate their own environment (e.g., _\ctxraits[....]{....}_ generates a Contexts Traits listing).


## Writing Conventions

* Inlined lists should be written using arabic numbers between parenthesis, e.g., (1), (2), ... This is defined using the \begin{enumerate*}[label=(\arabic*)] .. \end{enumerate*} environment.
* Always use \ac{ACRONYM} to refer to an acronym 
