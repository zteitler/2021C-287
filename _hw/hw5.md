---
layout: assignment
title: Homework 5
duedate: 2021-10-01
mathjax: true
---



This homework will be on Chapter 5.

**LaTeX:** This week we'll look at the distinction between
*inline* mathematics and *display* mathematics.

Please create a LaTeX document with the following code.

```
\documentclass[12pt,oneside]{amsart}

\title{Math 287 Homework 5}
\author{your name}
\date{October 10, 2021} % the due date of the homework

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


1.  This is a LaTeX exercise to learn about the distinction between *inline* mathematics
    versus *display* mathematics.
    
    The key distinctions are
    
    1.  Inline math is shown within a line of text. Display math is shown on its own line, centered.
    2.  Inline math is usually smaller (to fit within a line). Display math is usually bigger.
    3.  Display math can be numbered, or unnumbered. The numbers are so that you can refer back to the equation later
        (like "by equation (5) we get...").
    
    Inline mathematics like $$ e^{\pi i} + 1 = 0 $$ or \\( a^2 + b^2 = c^2 \\)
    can be typed in a couple of ways,
    including `$e^{\pi i} + 1 = 0$` or `\( a^2 + b^2 = c^2 \)`.
    Notice how `$...$` and `\(...\)` both are ways to declare "math mode",
    specifically inline math mode.
    
    Display mathematics like
    \\[ x = \frac{-b \pm \sqrt{b^2-4ac}}{2a} \\]
    or
    \\[ \int x^n \, dx = \frac{1}{n+1} x^{n+1} + C \\]
    can also be typed in a couple of ways,
    including `$$...$$` and `\[....\]`.
    These specific equations are
    `$$ x = \frac{-b \pm \sqrt{b^2-4ac}}{2a} $$`
    and `\[ \int x^n \, dx = \frac{1}{n+1} x^{n+1} + C \]`.
    
    Display mathematics can be numbered, or unnumbered.
    A numbered example is
    \\[ \cos^2(\theta)+\sin^2(\theta)=1. \tag{1} \\]
    If you want a numbered equation, the basic way to create one is
    `\begin{equation}...\end{equation}`.
    This specific example is
    `\begin{equation} \cos^2(\theta) + \sin^2(\theta) = 1 \end{equation}`.
    
    Unnumbered equations can be created with `$$...$$` or `\[...\]`
    or `\begin{equation*}...\end{equation*}`.
    
    Now, try using inline and display math in your homework!
    **Copy the following LaTeX code and paste it into your document**,
    between `\maketitle` and `\end{document}`:
    
    ```
    \begin{exer}
    Show some of your favorite equations in \emph{inline} and \textbf{display} mathematics.
    \end{exer}
    
    \begin{answer}
    Some people like small equations such as $e^{\pi i}+1 = 0$
    or \( a^2+b^2 = c^2 \).
    
    My favorite small equation is $...$.
    
    Other people like big equations like $$ x = \frac{-b \pm \sqrt{b^2-4ac}}{2a} $$
    and \[ \int x^n \, dx = \frac{1}{n+1} x^{n+1} + C . \]
    
    My favorite big equation is
    \[ ... \]
    \end{answer}
    ```
    
    **Fill in two of your favorite equations (or formulas)!**
    Delete the `...`'s and replace them with your equations/formulas.
    
    (You won't be graded on which equations/formulas you choose, as long as you manage to show
    an inline equation/formula and a display equation/formula.)


2.  **Project 5.16(ii).**
    
    Copy the following LaTeX code and paste it into your document:
    
    ```
    \newpage
    \begin{exer}
    Project 5.16(ii). Prove or give a counterexample: For all sets $A,B,C$,
    $A \cap (B-C) = (A \cap B) - (A \cap C)$.
    \end{exer}

    \begin{answer}
    -enter your answer here-
    \end{answer}
    ```
    
    If you believe the equation is true for all sets, give a proof.
    If you believe it is not true for all sets, give a counterexample.
    
    *Hint:* To figure out if the equation is true or not,
    try making up some random sets $$A,B,C$$ and working out each side of the equation
    to see if they match or not.
    
    **LaTeX:** Observe:
    +   The symbol for *intersection* of sets is $$\cap$$, typed `\cap`.
    
    +   The symbol for *union* of sets is $$\cup$$, typed `\cup`.


3.  **Proposition 5.20(ii).**
    
    Prove: If $$A,B,C$$ are any sets,
    then $$A \times (B \cap C) = (A \times B) \cap (A \times C)$$.
    
    (You don't have to test whether this is true or not,
    or figure out whether to give a counterexample.
    This is a true statement and you are being asked to give a proof.)


4.  **Project 5.21(ii).**
    
    (Prove or disprove. If you believe the equation is true, give a proof.
    If you believe it is not true for all sets, give a counterexample.
    You can try making up some random sets and working out each side of the equation
    to see if they match or not.)


5.  Find $$\sum_{j=0}^k f_j^2$$,
    where the $$f_j$$ are Fibonacci numbers as defined in the textbook.
    Prove your answer.
    
    Your answer will have a clear statement: $$\sum_{j=0}^k f_j^2 =$$ (your answer).
    Then, a proof of your answer.
    
    For your proof, use induction.
    
    For example, since the Fibonacci numbers start with $$0,1,1,2,3,5,8,\dotsc$$,
    you will get values starting with $$0^2=0$$, $$0^2+1^2=1$$, $$0^2+1^2+1^2=2$$,
    $$0^2+1^2+1^2+2^2=6$$, and so on.
    
    *Hint:* Work out some of the values and look for a pattern.
    It might be helpful to look at factorizations of the values.



##  Additional assignments, required

These items are assigned and required.
You do not have to turn in anything.
These items will not be graded.

+   Read Chapters 6 and 7 of the textbook.

+   Visit the [resources page]({{ "/resources" | relative_url }}) for this course.

+   Visit the Math Department's [tutoring page](https://www.boisestate.edu/math/academics/tutoring/#math-265-287-305-314-361)
    to learn about drop-in tutoring for this course.


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

+   Visit the Math Department's [research page](https://www.boisestate.edu/math/research/).
    Especially, take a look at the Math Department Colloquium (you are welcome to come to the talks!)
    and at the senior thesis projects posted in the Senior Showcase.
