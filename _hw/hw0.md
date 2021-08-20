---
layout: assignment
title: Homework 0
duedate: 2021-08-27
mathjax: true
---



This homework will be about establishing procedures:
using LaTeX to create a PDF,
and uploading that PDF to [Gradescope](https://gradescope.com).

+ For you to practice using LaTeX
+ For you to practice uploading an assignment to Gradescope
+ For me to practice working with a grader in Gradescope


## Problems

+   Read the course [syllabus]({{"/syllabus" | relative_url}}). (You don't need to turn in anything for this.)

+   Get access to LaTeX. If you already have this installed on your computer,
    or if you use a campus computer with LaTeX installed, then you don't need to do anything.
    You might want to download and install LaTeX
    ([MacTeX](http://www.tug.org/mactex/), [MikTex](https://miktex.org), or <https://www.latex-project.org/get/>),
    but that can be a very large download and possibly a lot of work.
    If you're new to LaTeX then I recommend starting with
    [Overleaf](https://www.overleaf.com/), a free online service.

1.  Create a LaTeX document with
    
    ```
    \documentclass[12pt,oneside]{amsart}

    \title{Math 287 Homework 0}
    \author{your name}
    \date{August 27, 2021} % the due date of the homework

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

    I made a \LaTeX~ document for my homework!

    \end{document}
    ```
    
    Copy that, and paste it into your LaTeX document.
    Change "your name" in the `author` line to be, well, your name.
    
    Take a look at your document now, before you do the rest of the homework.
    You might need to "compile" it.
    You should get a 1-page PDF.
    Did it work? Congratulations, you've made a LaTeX document!
    (If it didn't work, please email me and tell me what you tried,
    and what happened, including any error messages that came up.)
    
    The rest of this homework will add some more pages.

2.  (About yourself) Answer the questions. This will not be graded for correctness.
    The goal is just to tell me a little bit about yourself
    (and also to practice using LaTeX's enumerate lists).
    
    Add this to your LaTeX document (right before the `\end{document}`):
    
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
    \begin{answer}
    \begin{enumerate}
    \item My ``official'' name is...
    \item Please call me...
    \item
    \item
    \end{enumerate}
    \end{answer}
    ```
    
    **NOTE:** Please be aware that your answers will be viewed by the homework grader.
    They will be treated confidentially.
    However if you have anything sensitive that you want to communicate to me privately,
    then you might want to send that to me in an email
    or schedule an appointment to talk with me one-on-one.

3.  (About LaTeX) Have you used TeX or LaTeX before?
    
    Add this to your LaTeX document (after the previous answer, right before the `\end{document}`):
    
    ```
    \newpage
    \begin{exer}
    Have you used \TeX~ or \LaTeX~ before?
    \end{exer}

    \begin{answer}
    -enter your answer here-
    \end{answer}
    ```
4.  Add this to your LaTeX document (after the previous answer, right before the `\end{document}`):
    
    ```
    \newpage
    \begin{exer}
    Simplify $(x+y)^2 - (x-y)^2$.
    \end{exer}
    \begin{answer}
    $(x+y)^2 - (x-y)^2 = ...$ (enter your answer here)
    \end{answer}
    ```

5.  An example of a math joke is: What's a mathematician's favorite type of snake?
    Answer: an adder.
    
    Please share a math joke you like.
    
    Add this to your LaTeX document (after the previous answer, right before the `\end{document}`):
    
    ```
    \newpage
    \begin{exer}
    Please share a math joke.
    \end{exer}

    \begin{answer}
    -enter your math joke here-
    \end{answer}
    ```


+   Read Chapter 1 and Chapter 2 of the textbook.

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

You are encouraged to work together on the homework!


## Additional reading

+   Visit the Mathematics Colloquium web page: <https://www.boisestate.edu/math/research/colloquium/>

    You are invited to attend colloquium talks!

+   You might enjoy some YouTube math channels
    such as [3Blue1Brown](https://youtu.be/HEfHFsfGXjs)
    and [Mathologer](https://youtu.be/rGlpyFHfMgI).

