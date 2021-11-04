---
layout: assignment
title: Homework 8
duedate: 2021-11-06
mathjax: true
---



This homework will be on Chapter 9.

**LaTeX:** You'll learn how to type matrices, and, by popular request, margin notes.

Please create a LaTeX document with the following code.

```
\documentclass[12pt,oneside]{amsart}

\title{Math 287 Homework 8}
\author{your name}
\date{November 6, 2021} % the due date of the homework

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


1.  This is a LaTeX exercise about matrices and margin notes.
    
    Sometimes matrices are written with parentheses (round) around them, like this:
    
    ```
    \[
      \begin{pmatrix}
        a & b \\
        c & d \\
      \end{pmatrix}^{-1}
      =
      \frac{1}{ad-bc}
      \begin{pmatrix}
        d & -b \\
        -c & a \\
      \end{pmatrix}
    \]
    ```
    
    $$
      \begin{pmatrix}
        a & b \\
        c & d \\
      \end{pmatrix}^{-1}
      =
      \frac{1}{ad-bc}
      \begin{pmatrix}
        d & -b \\
        -c & a \\
      \end{pmatrix}
    $$
    
    And sometimes matrices are written with brackets (square) around them.
    This example equation shows the *determinant* of a $$2 \times 2$$ matrix:
    
    ```
    \[
      \det \begin{bmatrix}
        a & b \\
        c & d \\
      \end{bmatrix}
      = ad - bc
    \]
    ```
    
    $$
      \det \begin{bmatrix}
        a & b \\
        c & d \\
      \end{bmatrix}
      = ad - bc
    $$
    
    Observe:
    
    + Matrices are created within a math mode.
      (In these examples, the `\[...\]` creates display math.
      You could use `$$...$$`, `\begin{equation}...\end{equation}`, etc.
      You could even use `$...$` for inline math mode, although look out,
      because putting matrices like, for example, $$M = \begin{pmatrix} 1 & x & x^2 \\ 1 & y & y^2 \\ 1 & z & z^2 \end{pmatrix}$$
      within inline mode tends to cause the text lines to spread out a lot,
      just to make room for the matrix.
      (A big matrix like that might be better in display mode.)
    
    + All the entries of a matrix are automatically in math mode.
    
    + The rows of a matrix are separated with `\\`. The entries of a matrix within each row are separated with `&`.
    
    + Determinant is typed `\det`.
    
    
    **Margin notes:**
    There are several ways to make margin notes in LaTeX.
    Here are two of the ways:
    
    1.  The built-in command `\marginpar{...}` creates a basic margin note.
        For example, `\marginpar{I got hints for this homework problem from my study group.}`
        You can control which side it goes on: `\marginpar[one side]{}`, `\marginpar{other side}`.
        If you just want relatively simple margin notes, this might be good enough.
    
    2.  The `todonotes` package is much more powerful and customizable, including adding color to the notes.
        Add `\usepackage{todonotes}`, then you can create notes like
        `\todo{I haven't proofread this yet}`.
        There are lots of options, such as `\todo[color=green]{a green note}`
        or `\todo[inline]{a note inline, within your text}`.
    
    
    Your assignment:
    **Type the matrices with Fibonacci numbers and find their determinants.**
    Type these matrices in your document and find their determinants:
    
    $$
      \begin{pmatrix} 1 & 1 \\ 1 & 2 \end{pmatrix},
      \quad
      \begin{pmatrix} 1 & 2 \\ 2 & 3 \end{pmatrix},
      \quad
      \begin{pmatrix} 2 & 3 \\ 3 & 5 \end{pmatrix},
      \quad
      \begin{pmatrix} 3 & 5 \\ 5 & 8 \end{pmatrix},
      \quad
      \begin{pmatrix} 5 & 8 \\ 8 & 13 \end{pmatrix}
    $$
    
    Observe the pattern: the entries are Fibonacci numbers.
    
    To help you start,
    you can use this LaTeX code:
    
    ```
    We need to find the determinants of these matrices:
    \[
      \begin{pmatrix} 1 & 1 \\ 1 & 2 \end{pmatrix},
      ...
    \]
    The determinants are
    \[
      \det \begin{pmatrix} 1 & 1 \\ 1 & 2 \end{pmatrix} = ...,
    \]
    next
    \[
      ...
    \]
    ```
    
    (Optional (you do not need to turn in): Can you tell what are the next couple of matrices in this sequence?
    What are their determinants? Can you find a pattern?)
    
2.  **Proposition 9.7(ii)**
    
    LaTeX: The composition sign is made with `\circ`,
    for example `$g \circ f$` makes $$g \circ f$$.
    
    **Note:** A proof for this was given in class.
    For the homework assignment you can find a proof yourself,
    or you can rewrite and explain the class proof in your own words.



3.  **Claims:** Prove the claims:
    
    1.  For any $$n \geq 2$$, if $$f_1,f_2,\dotsc,f_n$$ are each injective,
        then $$f_1 \circ f_2 \circ \dotsb \circ f_n$$ is injective.
        
    2.  For any $$n \geq 2$$, if $$f_1,f_2,\dotsc,f_n$$ are each surjective,
        then $$f_1 \circ f_2 \circ \dotsb \circ f_n$$ is surjective.
    
    3.  For any $$n \geq 2$$, if $$f_1,f_2,\dotsc,f_n$$ are each bijective,
        then $$f_1 \circ f_2 \circ \dotsb \circ f_n$$ is bijective.
    
    (Hint: Use induction and Proposition 9.7.)
    
    LaTeX: Dots in a comma list are created with `\dotsc`,
    for example `$1,2,\dotsc,10$` makes $$1,2,\dotsc,10$$.
    Dots in a sequence of operations are created with `\dotsb`,
    for example `$1+2+\dotsb+10$` makes $$1 + 2 + \dotsb + 10$$.
    
    
    
4.  **Claims:** Suppose $$f: A \to B$$ and $$g: B \to C$$,
    so $$g \circ f$$ is a function $$A \to C$$.
    Prove the following claims:
    
    1.  If $$g \circ f$$ is injective, then $$f$$ is injective.
    
    2.  If $$g \circ f$$ is surjective, then $$g$$ is surjective.
        
        (Hint: For any $$c \in C$$, you want to show there's a $$b \in B$$ such that $$g(b) = c$$.
        The hypothesis tells you that there exists some $$a \in A$$ such that $$(g \circ f)(a) = c$$.)
    
    3.  If $$g \circ f$$ is bijective, then $$f$$ is injective and $$g$$ is surjective.
        Explain why (use the previous claims) and
        give an example to show that $$f$$ doesn't have to be surjective and $$g$$ doesn't have to be injective.
        
        (Hint: Give an example where $$f$$ is a function from a set with $$2$$ elements
        to a set with $$3$$ elements, and $$g$$ is from the set with $$3$$ elements
        back to a set with $$2$$ elements, such as $$f: \{1,2\} \to \{11,12,13\}$$
        and $$g: \{11,12,13\} \to \{21,22\}$$.
        Even with this hint, you still have to state some specific $$f$$ and $$g$$
        and explain why they satisfy what the example is asking for.)
    


##  Additional assignments, required

These items are assigned and required.
You do not have to turn in anything.
These items will not be graded.

+   Read Chapters 10-11 of the textbook.



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

+ Visit the [TeX Stack Exchange](https://tex.stackexchange.com) for questions and answers
  about TeX and LaTeX.


