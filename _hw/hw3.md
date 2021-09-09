---
layout: assignment
title: Homework 3
duedate: 2021-09-17
mathjax: true
---



This homework will be on Chapter 3.
This assignment has 4 problems instead of 5 like the last few homeworks.

**LaTeX:** This week we'll work with *lists* in our document.
There was a list before, in Homework 0 (for the questions about yourself),
so this will be your second chance to try using lists.

Please create a LaTeX document with the following code.
This week we're adding the `enumitem` package to give us some additional list options.

```
\documentclass[12pt,oneside]{amsart}

\title{Math 287 Homework 3}
\author{your name}
\date{September 17, 2021} % the due date of the homework

\usepackage[T1]{fontenc}
\usepackage{amsmath,amsfonts,amssymb,amsthm}
\usepackage[letterpaper,margin=1.5in]{geometry}
\usepackage{fancyhdr}
\pagestyle{fancy}
\usepackage{enumitem}

% Extra space between lines
\linespread{2.4}

\theoremstyle{remark}
\newtheorem{exer}{Exercise}
\newtheorem{claim}{Claim}[exer]

\newcommand{\bfN}{\mathbf{N}}
\newcommand{\bfZ}{\mathbf{Z}}


\newenvironment{answer}{\bigskip\noindent\emph{Answer.}}{\hfill$\diamond$\newline}

\begin{document}
\maketitle




\end{document}
```

Copy that, and paste it into your LaTeX document.
Change "your name" in the `author` line to be your name.



## Problems



1.  **Project 3.1 parts (iii)-(iv).**
    
    (We did parts (i)-(ii) in class.)
    
    To start, copy the following LaTeX code and paste it into your document,
    between `\maketitle` and `\end{document}`:
    
    ```
    \newpage
    \begin{exer}
    Project 3.1. Express each of the following statements using quantifiers.
    \begin{enumerate}[label={(\roman*)},start={3}]
    \item Every integer is the product of two integers.
    \item The equation $x^2-2y^2 = 3$ has an integer solution.
    \end{enumerate}
    \end{exer}

    \begin{answer}
    \begin{enumerate}[label={(\roman*)},start={3}]
    \item -enter your answer here-
    \item -enter your answer here-
    \end{enumerate}
    \end{answer}
    ```
    
    **LaTeX:** Numbered lists can be created with `enumerate`,
    and each item is created by an `\item` command.
    If you're familiar with HTML this is like `<ol>` for an ordered list
    `<li>` for each list item.
    
    Observe that we set the *label* of our lists using `(\roman*)` to make it use Roman numerals,
    and parentheses (just to match the textbook).
    We could have used other formats and punctuation, e.g., `label={\Alph*:}` to get `A:, B:, C:,...`.
    There are many more options, described in the `enumitem` documentation.

2.  **Project 3.2 parts (iii)-(iv).**
    
    To help you get started, you can copy this LaTeX code:
    ```
    \newpage
    \begin{exer}
    Project 3.2. In each of the following cases explain what is meant by the statement
    and decide whether it is true or false.
    \begin{enumerate}[label={(\roman*)},start={3}]
    \item For each $x \in \mathbf{Z}$ there exists $y \in \mathbf{Z}$ such that $xy=x$.
    \item There exists $y \in \mathbf{Z}$ such that for each $x \in \mathbf{Z}$, $xy=x$.
    \end{enumerate}
    \end{exer}

    \begin{answer}
    \begin{enumerate}[label={(\roman*)},start={3}]
    \item -enter your answer here-
    \item -enter your answer here-
    \end{enumerate}
    \end{answer}
    ```

3.  **Project 3.7 parts (iv)-(vii).**
    
    To help you get started, you can copy this LaTeX code:
    ```
    \newpage
    \begin{exer}
    Project 3.7. Negate the following statements.
    \begin{enumerate}[label={(\roman*)},start={4}]
    \item The newspaper article was neither accurate nor entertaining.
    \item If $\gcd(m,n)$ is odd, then $m$ or $n$ is odd.
    \item (you can enter this one)
    \item For each $\varepsilon > 0$ there exists $N \in \mathbf{N}$ such that
    for all $n \geq N$, $|a_n-L| < \varepsilon$.
    \end{enumerate}
    \end{exer}

    \begin{answer}
    \begin{enumerate}[label={(\roman*)},start={4}]
    \item -enter your answer here-
    \item -enter your answer here-
    \item
    \item
    \end{enumerate}
    \end{answer}
    ```
    
    **LaTeX:** We can use an underscore `_`
    (on most keyboards, press the Shift key and the `-` (minus) key)
    in order to produce subscript text such as `$a_n$`, $$a_n$$; or `$f_v(p)$`, $$f_v(p)$$.
    It can be combined with superscripts, e.g., `$x_m^2$`, $$x_m^2$$.
    
    
4.  Prove, using induction: For all $$k \in \mathbf{N}$$, $$5^k+3$$ is divisible by $$4$$.
    
    Make sure you remember the definition of "divisible" from page 7 of the textbook.
    We say $$m$$ is divisible by $$n$$ if there is some integer $$j$$ such that $$m=jn$$.
    In this case, saying that $$5^k+3$$ is divisible by $$4$$ means that $$5^k+3 = 4j$$
    for some integer $$j$$.
    
    To help you get started, you can copy this LaTeX code:
    ```
    \newpage
    \begin{exer}
    For all $k \in \mathbf{N}$, $5^k + 3$ is divisible by $4$.
    \begin{enumerate}
    \item Write what this statement says for $k=1$. Is it true or false? Explain.
    \item Write what this statement says for $k=2$. Is it true or false? Explain.
    \item Write what this statement says for $k=3$. Is it true or false? Explain.
    \end{enumerate}
    Now, prove the statement for all $k \in \mathbf{N}$, using induction.
    \end{exer}

    \begin{proof}
    \begin{enumerate}
    \item For $k=1$, the statement says that $5^1+3$ is divisible by $4$.
    It's true because $5+3=8$, and $8 = 4 \cdot 2$.
    \item
    \end{enumerate}
    -enter your proof here-
    \end{proof}
    ```
    
    **Hint:** How can we get from $$5^k$$ to $$5^{k+1}$$? What operation can we do to $$5^k$$
    to make it into $$5^{k+1}$$?
    
    **LaTeX:** Typing `$5^k$` gives you $$5^k$$, but how do you get $$5^{k+1}$$?
    If you try `$5^k+1$` you will get $$5^k+1$$ instead of $$5^{k+1}$$.
    
    To get $$5^{k+1}$$, you will need to group together the `k+1`
    using braces (`{...}`) like this: `$5^{k+1}$`.

##  Additional assignments, required

These items are assigned. Please do them!
But you do not have to turn in anything.
These items will not be graded.

+   Read Chapter 4 of the textbook. This is a longer chapter.


## Instructions

Use LaTeX to create a PDF. Upload your PDF to Gradescope.
If you don't have LaTeX on your computer, you can use [Overleaf](https://overleaf.com).
Don't submit the LaTeX source, just the PDF.
Email your instructor (that's me) if you have questions or need help.

Please include your name and the homework number within the document.
Some additional formatting instructions are in the
[syllabus]({{ "/syllabus" | relative_url }}).
To summarize:

+ Use a new page (`\newpage`) for each problem.
+ State which question you are answering and the actual question.
  Then, start your answer in a new paragraph.

You are encouraged to work together on the homework!


## Additional assignments, optional

These are optional (not required).

+   Watch <https://youtu.be/N-KXStupwsc>
    "500 years of NOT teaching THE CUBIC FORMULA.
    What is it they think you can't handle?" by Mathologer (length: 36:57).

+   Watch <https://www.youtube.com/watch?v=EK32jo7i5LQ>
    "Why do prime numbers make these spirals?" by 3Blue1Brown (length: 22:29).
    Please be an engaged, active watcher--try to think about and understand
    what you're watching, not just let it go by.

