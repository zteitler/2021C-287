---
layout: assignment
title: Homework 4
duedate: 2021-09-24
mathjax: true
---



This homework will be on Chapter 4.

**LaTeX:** This week we'll see how to type *summations*.

Please create a LaTeX document with the following code.

```
\documentclass[12pt,oneside]{amsart}

\title{Math 287 Homework 4}
\author{your name}
\date{September 24, 2021} % the due date of the homework

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


1.  **Explain the proof of Proposition 4.6(ii).**
    The textbook gives a proof of Proposition 4.6(ii).
    Rewrite the proof in more detail and with more explanation.
    

2.  **Proposition 4.7 part (iii).**
    
    To start, copy the following LaTeX code and paste it into your document,
    between `\maketitle` and `\end{document}`:
    
    ```
    \newpage
    \begin{exer}
    Proposition 4.7(iii). For all $k \in \mathbf{N}$,
    $10^k + 3 \cdot 4^{k+2} + 5$ is divisible by $9$.
    \end{exer}

    \begin{proof}
    -enter your proof here-
    \end{proof}
    ```
    
    Use proof by induction, even if you know another approach that could work.
    The purpose here is to learn and practice induction proofs.
    
    **LaTeX:** Observe:
    +   The math symbol for a multiplication dot is `\cdot`, $$\cdot$$.
        This makes a "centered dot" (the "c" is for "centered").
        
    +   Observe that we used braces, `{...}`, to group together the power
        `4^{k+2}`, $$4^{k+2}$$.
        When you need to type a power like $$4^{k+2}$$, $$10^{k+1}$$, $$4^{k+3}$$, etc.,
        with more than just one number or letter in the power,
        use the braces (`4^{k+2}`, `10^{k+1}1`, `4^{k+3}`, etc).

3.  **Project 4.9.**
    
    In this problem you will (1) determine for which natural numbers the statement is true,
    and (2) prove your answer.
    In your answer, you should state very clearly which natural numbers make the statement true:
    something like "For all natural numbers $$k$$ such that (your answer here), $$k^2 < 2^k$$."
    Or you could phrase it differently, for example, as "If $$k$$ is (your answer here), $$k^2 < 2^k$$."
    You will have to fill in what condition is needed for the $$k$$.
    Then, prove your statement.
    
    To find the right condition, please try some $$k$$ values.
    Try $$k=1,2,3,\dotsc$$ (we are talking about natural numbers so it makes sense to count up from 1).
    Which $$k$$ values make $$k^2 < 2^k$$ true?


4.  Find $$\sum_{j=0}^k f_j$$, where the $$f_j$$ are Fibonacci numbers as defined in the textbook.
    Prove your answer.
    
    **Hint:** Try $$\sum_{j=0}^k f_j$$ for several values of $$k$$
    (e.g., $$k=1,2,3,\dotsc,6,\dotsc$$). Look for a pattern.
    
    **LaTeX:** A summation symbol is typed with `\sum`, $$\sum$$.
    We use a subscript to show the starting point of the summation:
    `\sum_{j=0}`, $$\sum_{j=0}$$.
    We can add a superscript to show the ending point of the summation:
    `\sum_{j=0}^k`, $$\sum_{j=0}^k$$.




##  Additional assignments, required

These items are assigned. Please do them!
But you do not have to turn in anything.
These items will not be graded.

+   Read Chapters 5 and 6 of the textbook.


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

+   [Considering graduate school in mathematics?](https://www.ams.org/education/pre-grad)

+   Check out summer [Research Experiences for Undergraduates (REUs)](https://www.ams.org/programs/students/emp-reu)

+   More [student resources and information](https://www.maa.org/member-communities/students)
