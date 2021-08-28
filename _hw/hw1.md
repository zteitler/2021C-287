---
layout: assignment
title: Homework 1
duedate: 2021-09-03
mathjax: true
---



This homework will be on Chapter 1.

For this homework we will once again use some of the LaTeX code from [Homework 0]({{ "/hw/hw0" | relative_url }}).
Please create a LaTeX document with the following code.

```
\documentclass[12pt,oneside]{amsart}

\title{Math 287 Homework 1}
\author{your name}
\date{September 3, 2021} % the due date of the homework

\usepackage[T1]{fontenc}
\usepackage{amsmath,amsfonts,amssymb,amsthm}
\usepackage[letterpaper,margin=1.5in]{geometry}

% Extra space between lines
\linespread{2.4}

\theoremstyle{remark}
\newtheorem{exer}{Exercise}

\newenvironment{answer}{\bigskip\noindent\emph{Answer.}}{\hfill$\diamond$\newline}

\begin{document}
\maketitle




\end{document}
```

Copy that, and paste it into your LaTeX document.
Change "your name" in the `author` line to be your name.



## Problems

This is a list of problems from the textbook, given by reference number.
Your homework is to write a proof of the statement.

1.  Proposition 1.11(vi).
    
    In other words, please write a proof of Proposition 1.11(vi).
    To start, copy the following LaTeX code and paste it into your document,
    between `\maketitle` and `\end{document}`:
    
    ```
    \newpage
    \begin{exer}
    Proposition 1.11(vi). If $m$, $n$, $p$, and $q$ are integers, then
    $(m(n+p))q = (mn)q + m(pq)$.
    \end{exer}

    \begin{proof}
    -enter your proof here-
    \end{proof}
    ```
    
    Please observe:
    
    + We indicate which textbook problem it is (Proposition 1.11(vi))
      and give a clear statement of what we are supposed to prove.
      
    + The proof is inside a `\begin{proof}...\end{proof}`.
    
    

2.  Proposition 1.22(i).
    
    To help you get started, you can copy this LaTeX code:
    ```
    \newpage
    \begin{exer}
    Proposition 1.22(i). For all $m \in \mathbf{Z}$, $-(-m) = m$.
    \end{exer}
    
    \begin{proof}
    -enter your proof here-
    \end{proof}
    ```
    
    For exercises in this class we should only use theorems and axioms
    that are stated *before* the problem we're trying to solve.
    So, for this problem you should only use statements from Corollary 1.21 or earlier.
    
    Hint: One way to prove this statement is to use Proposition 1.10
    with $$-(-m)$$ and $$m$$ substituted for $$x_1$$ and $$x_2$$,
    and $$-m$$ substituted for $$m$$.
    If you do this, or if you find a different proof,
    make sure you explain your proof (it should make sense for someone who
    hasn't read this hint).


3.  Proposition 1.22(ii).

4.  Proposition 1.20. In this problem, the textbook gives a proof.
    Your homework is to explain the proof in more detail.

5.  Proposition 1.14.
    
    Hint: $$0 = 0+0$$.


+   Read Chapter 2 and Chapter 3 of the textbook.

## Instructions

Use LaTeX to create a PDF. Upload your PDF to Gradescope.
If you don't have LaTeX on your computer, you can use [Overleaf](https://overleaf.com).
Don't submit the LaTeX source, just the PDF.
Email your instructor (that's me) if you have questions or need help.

Please include your name and the homework number
(this is Homework 1) within the document.
Some additional formatting instructions are in the
[syllabus]({{ "/syllabus" | relative_url }}).
To summarize:

+ Use a new page (`\newpage`) for each problem.
+ State which question you are answering and the actual question.
  Then, start your answer in a new paragraph.

You are encouraged to work together on the homework!


## Additional reading

+   Some math career info is linked from my webpage at <https://zteitler.github.io/links/>.

+   Check out [Theorem of the Day](https://www.theoremoftheday.org)!
