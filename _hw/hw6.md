---
layout: assignment
title: Homework 6
duedate: 2021-10-08
mathjax: true
---



This homework will be on Chapter 6.

**LaTeX:** This week we'll learn a way to *align* display math.

Please create a LaTeX document with the following code.

```
\documentclass[12pt,oneside]{amsart}

\title{Math 287 Homework 6}
\author{your name}
\date{October 8, 2021} % the due date of the homework

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


1.  This is a LaTeX exercise to learn a way to *align* display math.
    Aligning means that multiple lines or equations are lined up below each other.
    This can be useful for showing several equations or for showing
    multiple steps in a problem.
    Here are two examples.
    
    First, here's an example that shows multiple steps:
    
    $$
    \begin{split}
      10^{k+1} + 3 \cdot 4^{k+1+2} + 5 &= 10 \cdot 10^k + 3 \cdot 4 \cdot 4^{k+2} + 5 \\
        &= 10 \cdot 10^k + 12 \cdot 4^{k+2} + 5 \\
        &= (1 + 9) \cdot 10^k + (3 + 9) \cdot 4^{k+2} + 5 \\
        &= 10^k + 9 \cdot 10^k + 3 \cdot 4^{k+2} + 9 \cdot 4^{k+2} + 5 \\
        &= (10^k + 3 \cdot 4^{k+2} + 5) + (9 \cdot 10^k + 9 \cdot 4^{k+2}) \\
        &= (10^k + 3 \cdot 4^{k+2} + 5) + 9 (10^k + 4^{k+2})
    \end{split}
    $$
    
    Can you follow along and see what was done in each step?
    
    Here's another example:
    
    $$
    \begin{split}
      2^{k+1} &= 2 \cdot 2^k \\
        &> 2 \cdot k^2 \qquad \text{because of induction hypothesis $k^2<2^k$} \\
        &= k^2 + k^2 \\
        &= k^2 + k \cdot k \\
        &> k^2 + 3k \qquad \text{because of hypothesis $k \geq 5$} \\
        &= k^2 + 2k + k \\
        &> k^2 + 2k + 1 \\
        &= (k+1)^2
    \end{split}
    $$
    
    There are other ways of aligning equations, but this week we will focus on this one.
    
    Here are the LaTeX codes for those examples:
    
    ```
    \[
    \begin{split}
      10^{k+1} + 3 \cdot 4^{k+1+2} + 5 &= 10 \cdot 10^k + 3 \cdot 4 \cdot 4^{k+2} + 5 \\
        &= 10 \cdot 10^k + 12 \cdot 4^{k+2} + 5 \\
        &= (1 + 9) \cdot 10^k + (3 + 9) \cdot 4^{k+2} + 5 \\
        &= 10^k + 9 \cdot 10^k + 3 \cdot 4^{k+2} + 9 \cdot 4^{k+2} + 5 \\
        &= (10^k + 3 \cdot 4^{k+2} + 5) + (9 \cdot 10^k + 9 \cdot 4^{k+2}) \\
        &= (10^k + 3 \cdot 4^{k+2} + 5) + 9 (10^k + 4^{k+2})
    \end{split}
    \]
    ```
    
    and
    
    ```
    \[
    \begin{split}
      2^{k+1} &= 2 \cdot 2^k \\
        &> 2 \cdot k^2 \qquad \text{because of induction hypothesis $k^2<2^k$} \\
        &= k^2 + k^2 \\
        &= k^2 + k \cdot k \\
        &> k^2 + 3k \qquad \text{because of hypothesis $k \geq 5$} \\
        &= k^2 + 2k + k \\
        &> k^2 + 2k + 1 \\
        &= (k+1)^2
    \end{split}
    \]
    ```
    
    + This way of aligning uses a LaTeX environment called *split*,
      created using `\begin{split}...\end{split}`.
    
    + Each line in the split ends with `\\`.
    
    + Within each line there's a single alignment point, marked with an ampersand, `&`.
    
    + LaTeX aligns the equation lines so the alignment points are stacked vertically.
    
    + It's very, very common to align steps so that equals signs line up,
      by using split with `&=`.
      In the first example, every single step (after the first line) just had `&=`.
      
    + But you are allowed to align whatever you want.
      In the second example some steps were aligned on inequalities, using `&>`.
    
    + If you forget the line-ending `\\`, or include more than one alignment point `&`,
      then LaTeX will have some really weird errors.
      To fix it, just fill in the missing `\\` or take away the extra `&`.
    
    Your assignment is to try using `split`.
    
    **Complete this simplification.**
    (Fill in the ?'s. You might not need all of them, so delete the extras.)
    Copy the following LaTeX code and paste it into your document,
    between `\maketitle` and `\end{document}`:
    
    ```
    \newpage
    \begin{exer}
    The derivative of $x^2$ is $2x$.
    \end{exer}
    \begin{proof}
    Let $f(x) = x^2$.
    Using the limit definition of derivative, we have
    \begin{equation}
    \begin{split}
      \lim_{h \to 0} \frac{f(x+h) - f(x)}{h} &= ? \\
        &= ? \\
        &= ? \\
        &= ? \\
        &= ? \\
        &= ? \\
        &= ? \\
        &= ? \\
        &= ? \\
        &= ?
    \end{split}
    \end{equation}
    \end{proof}
    ```
    
    **Hint:** Start by replacing $$f(x)$$ with $$x^2$$ and $$f(x+h)$$ with $$(x+h)^2$$.
    Then multiply out $$(x+h)^2$$ and simplify.
    
    (*Optional challenge*: Can you use the limit definition of derivative
    to find the derivative of $$f(x) = \sqrt{x}$$, or $$g(x) = \frac{1}{x}$$?
    Can you show your steps in LaTeX?)

2.  **Project 6.9(i), transitive.**
    
    Prove that the relation defined in the book is transitive.
    
    There is one step in the middle of the proof
    where you will use the fact that the set is
    $$\mathbf{Z} \times (\mathbf{Z}-\{0\})$$,
    meaning that we are looking at pairs $$(m,n)$$ where $$n \neq 0$$.
    When you get to that step, in other words when you use the fact that $$n \neq 0$$,
    please highlight that and state it clearly.
    Say why it matters that $$n \neq 0$$.
    
    (**Hint:** It's because there's a step where we divide by $$n$$,
    but we can't divide by $$0$$. So, knowing $$n \neq 0$$ is important.
    Please show which step that is, and explain it in your own words.)
    
    **LaTeX:** The symbol that the book uses for the relation, $$\sim$$,
    is typed `\sim` (short for "similar").


3.  **Proposition 6.17.**
    
4.  **Explain the proof of Proposition 6.29(i).**
    The textbook gives a proof of Proposition 6.29(i).
    Rewrite the proof in more detail and with more explanation.

##  Additional assignments, required

These items are assigned and required.
You do not have to turn in anything.
These items will not be graded.

+   Read Chapter 7 of the textbook.

+   Review Chapters 1-6 of the textbook for our midterm exam.
    
    The midterm exam will be in class on Wednesday, October 13.
    More information will be shared soon.


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

+   Here's a video about [proof by induction](https://youtu.be/Bp6jbrkQf_4)

+   Here's a video about [modular arithmetic and some cool connections to other topics](https://youtu.be/qhbuKbxJsk8)


