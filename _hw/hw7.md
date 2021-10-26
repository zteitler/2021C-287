---
layout: assignment
title: Homework 7
duedate: 2021-10-29
mathjax: true
---



This homework will be on Chapter 8.

**LaTeX:** This week we'll learn about math equations with text mixed in.

Please create a LaTeX document with the following code.

```
\documentclass[12pt,oneside]{amsart}

\title{Math 287 Homework 7}
\author{your name}
\date{October 29, 2021} % the due date of the homework

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


1.  This is a LaTeX exercise to learn how to include words in math equations.
    
    The quick answer is the `\text{...}` command.
    For example,  
    
    `6\mathbb{Z} = \{ a \in \mathbb{Z} \mid a = 6b \text{ for some $b \in \mathbb{Z}$} \}`
    
    makes
    
    $$ 6\mathbb{Z} = \{ a \in \mathbb{Z} \mid a = 6b \text{ for some $b \in \mathbb{Z}$} \} $$
    
    With
    
    `\sup(S) = \text{ the smallest element of } \{ b \in \mathbb{R} \mid b \geq x \text{ for all $x \in S$} \}`
    
    we get
    
    $$\sup(S) = \text{ the smallest element of } \{ b \in \mathbb{R} \mid b \geq x \text{ for all $x \in S$} \}$$
    
    One more:
    
    ```
    |x| = \begin{cases}
      x & \text{if $x \geq 0$} \\
      -x & \text{otherwise}
    \end{cases}
    ```
    
    gives us
    
    $$
    |x| = \begin{cases}
      x & \text{if $x \geq 0$} \\
      -x & \text{otherwise}
    \end{cases}
    $$
    
    And one more.
    Adding text in equations is useful for showing explanations alongside steps of a calculation.
    For example:
    
    ```
    \begin{split}
    \sum_{j=0}^{n+1} f_j^2 &= \left( \sum_{j=0}^n f_j^2 \right) + f_{n+1}^2 \\
      &= ( f_n f_{n+1} ) + f_{n+1}^2 \qquad \text{by induction} \\
      &= f_{n+1}(f_n + f_{n+1}) \qquad \text{pulling out a common factor} \\
      &= f_{n+1} f_{n+2} \qquad \text{by the recursive definition of Fibonacci numbers} \\
    \end{split}
    ```
    
    $$
    \begin{split}
    \sum_{j=0}^{n+1} f_j^2 &= \left( \sum_{j=0}^n f_j^2 \right) + f_{n+1}^2 \\
      &= ( f_n f_{n+1} ) + f_{n+1}^2 \qquad \text{by induction} \\
      &= f_{n+1}(f_n + f_{n+1}) \qquad \text{pulling out a common factor} \\
      &= f_{n+1} f_{n+2} \qquad \text{by the recursion of Fibonacci numbers} \\
    \end{split}
    $$
    
    Notice:
    
    + The text doesn't line up. This can be fixed, but it's a story for another day.
    
    + It's not very good for long texts
    
    + This should be used sparingly (only a little bit).
      Most teachers will want you to write sentences for most steps of your proofs.
    
    **Exercise:** Type in this definition of the Fibonacci numbers:
    
    $$
    f_n = \begin{cases}
      0, & \text{if $n=0$}, \\
      1, & \text{if $n=1$}, \\
      f_{n-1} + f_{n-2} & \text{otherwise}
    \end{cases}
    $$
    
    (The exercise is to figure out the LaTeX code to make this equation.)

2.  **Proposition 8.18**


3.  **Proposition 8.32**
    
    Prove all four of the statements listed in the Proposition.
    
    Suggestion: Set up your work like
    
    ```
    \begin{claim}
    If $$x < y$$ then...
    \end{claim}
    \begin{proof}
    (Your proof)
    \end{proof}
    
    \begin{claim}
    If $$x<y$$ and $$z<w$$ then...
    \end{claim}
    \begin{proof}
    (Your proof)
    \end{proof}
    
    ...
    ```
    
    and so on, listing each claim along with its proof.
    
    For some of these proofs you might use the method shown above
    to write a text reason (such as "Axiom 8.2") next to steps
    in a multi-step calculation.
    
    
4.  **Proposition 8.53**  
    Hint: If $$M$$ is a lower bound for $$A$$, then
    define $$B = \{ -x \mid x \in A \}$$, show that $$-M$$ is an upper bound for $$B$$,
    and use Axiom 8.52.

##  Additional assignments, required

These items are assigned and required.
You do not have to turn in anything.
These items will not be graded.

+   Read Chapters 9-10 of the textbook.



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

+   TikZducks is [a package to draw little ducks in LaTeX documents](https://ctan.org/pkg/tikzducks?lang=en)  
    (Try adding `\usepackage{tikzducks}` in your document's preamble,
    and then putting `\begin{tikzpicture} \duck \end{tikzpicture}` in the body of your document.)

ICYMI (In Case You Missed It): repeating some links from previous assignments

+   [A Guide to Writing Mathematics](https://web.cs.ucdavis.edu/~amenta/w10/writingman.pdf)
    (Warning, this is 17 pages long! You might want to read just a little bit at a time.)

+   [Getting better at proofs](https://math.stackexchange.com/questions/7743/getting-better-at-proofs)

+   Non-academic careers:
    BIG stands for Business, Industry, and Government, and encompasses a wide range of careers
    that a math student might be interested in.
    Visit the [AMS BIG career page](http://www.ams.org/profession/career-info/big)
    and the [BIG Math Network](https://bigmathnetwork.org/).

+   Check out summer [Research Experiences for Undergraduates (REUs)](https://www.ams.org/programs/students/emp-reu)

+   More [student resources and information](https://www.maa.org/member-communities/students)

+   Visit the Math Department's [research page](https://www.boisestate.edu/math/research/).
    Especially, take a look at the Math Department Colloquium (you are welcome to come to the talks!)
    and at the senior thesis projects posted in the Senior Showcase.


