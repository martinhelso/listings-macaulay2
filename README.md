# Macaulay2 for listings

The file `lstlang0.sty` defines _Macaulay2_ as a language in the LaTeX package `listings`.

## Usage

Store `lstlang0.sty` in the working folder or in the same directory as the other `listings` files.

### Choice of language
The language can be set globally in the document with
```LaTeX
\lstset{language = Macaulay2}
```
It can be set locally with
```LaTeX
\lstinputlisting[language = Macaulay2]{filename}
```
or
```LaTeX
\begin{lstlisting}[language = Macaulay2]
    ...
\end{lstlisting}
```

### Formatting
The keywords are divided into the same four types as in the highlighting done by `emacs`. By default, all four types are typeset in the same style. You can choose an individual style for each type:
```LaTeX
\lstset
{
    keywordstyle = [1]\bfseries,
    keywordstyle = [2]\itshape,
    keywordstyle = [3]\sffamily,
    keywordstyle = [4]\color{blue},
}
```
