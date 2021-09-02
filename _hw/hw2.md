---
layout: assignment
title: Homework 2
duedate: 2021-09-10
mathjax: true
---



This homework will be on Chapter 2.

Please create a LaTeX document with the following code.

**Note:** This LaTeX code is not the same as in Homework 1.
We're gradually adding more to it.
This time, we've added: "fancy" page headers,
a "claim" setup, and shortcut commands for $$\mathbf{N}$$ and $$\mathbf{Z}$$.
You'll be able to type `\bfN` and `\bfZ` as shortcuts instead of `\mathbf{N}` and `\mathbf{Z}`.

```
\documentclass[12pt,oneside]{amsart}

\title{Math 287 Homework 2}
\author{your name}
\date{September 10, 2021} % the due date of the homework

\usepackage[T1]{fontenc}
\usepackage{amsmath,amsfonts,amssymb,amsthm}
\usepackage[letterpaper,margin=1.5in]{geometry}
\usepackage{fancyhdr}
\pagestyle{fancy}

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


**LaTeX:** The `\newcommand` in LaTeX can be used to define shortcuts and other commands.
In this homework template we're using it for the shortcuts `\bfN` and `\bfZ`.
Try defining your own shortcut commands!


## Problems

This is a list of problems from the textbook, given by reference number.
Your homework is to write a proof of the statement.

**Note:** In this class, to prove a statement,
you are allowed to use any statement (proposition, axiom, definition, etc.)
that is in the textbook before the statement you are trying to prove.
You can use previous-numbered statements even if they
weren't proved in class or on homework,
or if they were on the homework but you haven't done that problem yet.



1.  **Proposition 2.7(iv).**
    
    To start, copy the following LaTeX code and paste it into your document,
    between `\maketitle` and `\end{document}`:
    
    ```
    \newpage
    \begin{exer}
    Proposition 2.7(iv). Let $m,n,p,q \in \bfZ$.
    If $m < n$ and $p < 0$ then $np < mp$.
    \end{exer}

    \begin{proof}
    -enter your proof here-
    \end{proof}
    ```

2.  **Proposition 2.12(iii).**
    
    To help you get started, you can copy this LaTeX code:
    ```
    \newpage
    \begin{exer}
    Proposition 2.12(iii). For all $m,n,p \in \bfZ$,
    if $p < 0$ and $mp < np$ then $n < m$.
    \end{exer}

    \begin{proof}
    -enter your proof here-
    \end{proof}
    ```

3.  **Proposition 2.26.** In this problem, the textbook gives a proof.
    Your homework is to rewrite the proof in more detail.
    
    Imagine a student in the class is confused by the proof.
    Rewrite the proof in a way that would make sense and be clear
    for a confused student.


4.  **Project 2.28.**
    
    In this project, you are supposed to
    
    1.  Determine for which natural numbers $$k^2 - 3k \geq 4$$.
        As part of your homework, give a clear statement of your answer.
    
    2.  Prove your answer.
    
    To help you get started, you can copy this LaTeX code:
    ```
    \newpage
    \begin{exer}
    Project 2.28. Determine for which natural numbers $k^2 - 3k \geq 4$
    and prove your answer.
    \end{exer}

    \begin{answer}
    \begin{claim}
    $k^2 - 3k \geq 4$ for (enter which values of k work)
    \end{claim}

    \begin{proof}
    (enter your proof here)
    \end{proof}
    \end{answer}
    ```
    
    **LaTeX:** Observe, we can write squares (and other powers)
    using LaTeX code `k^2`, `k^3`, and so on.
    As an experiment, try writing `k^m+1` and `k^{m+1}`.
    The curly braces `{...}` group together terms in LaTeX.

5.  This homework problem has two parts:
    
    1.  **Project 2.35**, compute $$\gcd(-4,10)$$, using the definition on page 22,
        in terms of being the smallest element of the set of $$-4x+10y$$ with integer $$x$$ and $$y$$.
        
        (This means (1) state what the value of the gcd is, (2) show that your value
        is given as an integer combination of $$-4$$ and $$10$$,
        (3) show that your value is the smallest positive integer combination of $$-4$$ and $$10$$,
        in other words there's no smaller positive integer in the set of $$-4x+10y$$.)
        
        (Only $$\gcd(-4,10)$$, not the rest of the project.)
    
    2.  As a thought experiment, let's try defining "gcd of rational numbers" like this.
        Suppose $$a$$ and $$b$$ are rational numbers, take the set of elements $$ax+by$$
        where $$x$$ and $$y$$ are rational numbers, and $$ax+by > 0$$.
        Can we define "$$\gcd(a,b)$$" to be the smallest element of that set?
        Why or why not? Explain.


+   Read Chapter 3 and Chapter 4 of the textbook.

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


## Additional reading

+   [A Guide to Writing Mathematics](https://web.cs.ucdavis.edu/~amenta/w10/writingman.pdf)
    (Warning, this is 17 pages long! You might want to read just a little bit at a time.)

+   [Getting better at proofs](https://math.stackexchange.com/questions/7743/getting-better-at-proofs)

+   [Examples of unexpected mathematical images](https://mathoverflow.net/q/178139/88133)

+   Visit [AMS information about graduate programs](http://www.ams.org/education/pre-grad)

+   Non-academic careers:
    BIG stands for Business, Industry, and Government, and encompasses a wide range of careers
    that a math student might be interested in.
    Visit the [AMS BIG career page](http://www.ams.org/profession/career-info/big)
    and the [BIG Math Network](https://bigmathnetwork.org/).
