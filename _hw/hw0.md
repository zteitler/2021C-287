---
layout: assignment
title: Homework 0
duedate: 2021-08-27
mathjax: true
---



This homework will be about establishing procedures:
using LaTeX to create a PDF, and uploading that PDF to [Gradescope](https://gradescope.com);
and using WebWork.

+ For you to practice using LaTeX
+ For you to practice uploading an assignment to Gradescope
+ For me to practice working with a grader in Gradescope
+ For you to practice working with WebWork


## Problems

+   Read the course syllabus. (You don't need to turn in anything for this.)

1.  Read <http://web.stonehill.edu/compsci/History_Math/math-read.htm>.
    
    + What is one interesting or surprising idea you learned from this reading?
    
    + What is one idea you will use when you read mathematics?


2.  (LaTeX: Using "split" to align equations)
    Complete this simplification.
    Enter this LaTeX code into your tex file, and answer it.
    (Fill in the ?'s. You might not need all of them, so delete the extras.)
    
    ```
    \newpage
    \begin{exer}
    Expand and simplify $$\frac{1}{4}(x+y)^2 - \frac{1}{4}(x-y)^2$$.
    \end{exer}
    \begin{answer}
    By multiplying out and grouping like terms we get
    \begin{equation}
    \begin{split}
      \frac{1}{4}(x+y)^2 - \frac{1}{4}(x-y)^2 &= ? \\
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
    \end{answer}
    ```

3.  Binomial Theorem.
    
    + Review factorials (e.g., $$3! = 6$$) and binomial coefficients (e.g., $$\binom{5}{2} = 10$$).
      (You don't need to turn in anything for this.)
    
    + Review the binomial theorem, $$(x+y)^n = \sum_{i=0}^n \binom{n}{i} x^i y^{n-i}$$.
    
    1.  Expand: $$(x+y)^5$$, $$(2x-y)^4$$, $$(x+y+z)^3$$  
        (hint: one way is to use the binomial theorem for $$(x+(y+z))^3$$, then again for powers of $$(y+z)$$).
    
    2.  Expand and simplify:
        \\[ (x+y+z)^3 - (x+y-z)^3 - (x-y+z)^3 + (x-y-z)^3 \\]
    
    3.  Expand and simplify:
        \\[ (x+y)^4 + i(x+iy)^4 + i^2(x+i^2y)^4 + i^3(x+i^3y)^4 , \\]
        where $$i = \sqrt{-1} \in \mathbb{C}$$.
        (That is, $$i^2=-1$$. So we also have $$i^3=-i$$ and $$i^4=1$$.)



4.  Read [Self-Explanation Training for Mathematics Students](
    https://www.lboro.ac.uk/media/media/schoolanddepartments/mathematics-education-centre/downloads/research/SE-booklet.pdf).
    Write a self-explanation of Practice Proof 1.
    
    If you've already written a self-explanation of Practice Proof 1 (e.g., in one of my previous classes)
    then write a self-explanation of Practice Proof 2.


5.  (About yourself) Answer the questions. This will not be graded for correctness.
    The goal is just to tell me a little bit about yourself
    (and also to practice using LaTeX's enumerate lists).
    
    ```
    \newpage
    \begin{exer}
    \begin{enumerate}
    \item What is your ``official'' name as on the class roster?
    \item What name do you like to go by in class?
    \item How is your name pronounced?
    \item What pronouns do you prefer (this could be she/her/hers, he/him/his,
      they/them/theirs, or other)?
    \item What is something that you are excited to learn in this class?
    \item What is something that you are concerned about in this class?
    \item Is there anything else you would like me to know?
    \end{enumerate}
    \end{exer}
    ```

## Instructions

Use LaTeX to create a PDF. Upload your PDF to Gradescope.
If you don't have LaTeX on your computer, you can use [Overleaf](https://overleaf.com).
Don't submit the LaTeX source, just the PDF.
Email your instructor (that's me) if you have questions or need help.

Please include your name and the homework number
(this is Homework 0) within the document.
Some additional formatting instructions are in the
[syllabus]({{ "/syllabus" | relative_url }}).
To summarize:

+ Use a new page (`\newpage`) for each problem.
+ State which question you are answering and the actual question.
  Then, start your answer in a new paragraph.
+ Use environments such as `proof` and `theorem`
  (via `\begin{proof}...\end{proof}`).
+ Use 12pt option `\documentclass[12pt]{amsart}` and linespacing `\linespread{2.4}`.

Please find and use the [LaTeX template for homework]({{ "/assets/405505-Homework-template.tex" | relative_url }}).

You are encouraged to work together on the homework!


## Additional reading

+   Visit the Mathematics Colloquium web page: <https://www.boisestate.edu/math/research/colloquium/>

    Visit the Mathematics seminars web page: <https://www.boisestate.edu/math/research/seminars/>.
    Especially [TATERS](https://sites.google.com/boisestate.edu/taters/)
    will feature a lot of talks related to this class, including a talk by John Little, one of the textbook authors.

    You are invited to attend colloquium and seminar talks!

+   You might be interested in this paper about writing proofs:  
    <https://web.cs.ucdavis.edu/~amenta/w10/writingman.pdf>  
    But, warning, it’s pretty long, 17 pages. You might want to read a little bit at a time.

