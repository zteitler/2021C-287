---
layout: assignment
title: Homework 9
duedate: 2021-11-13
mathjax: true
---



This homework will be on Chapter 10.

**LaTeX:** We'll learn how to include a graphic.

Please create a LaTeX document using the code
that has been posted in previous homework assignments.
(Please update it to say Homework 9, with the correct due date,
and including your name.)



## Problems


1.  This is a LaTeX exercise to learn how to include a graphic. Follow the steps:
    
    1.  Find or create a graphic to include, that you want to share.
        It can be a math image that you like such as a cool plot or interesting diagram,
        or a picture of an important mathematician.
        Or it can be a meme or joke.
        It doesn't have to be math-related.
        However **all images must be completely appropriate for sharing.**
        Political, religious, offensive, lewd, provocative, or suggestive images are not appropriate
        for sharing in a class assignment.
        
        Save your graphic in a common image format such as `jpg` or `png`.
    
    2.  Upload the graphic file to your Overleaf project or, if you're using LaTeX on
        your own computer, save it in the same directory as your homework LaTeX file.
        For guidelines on this, see <https://www.overleaf.com/learn/how-to/Including_images_on_Overleaf>.
    
    3.  Add the following line to your LaTeX source file:
        
        `\usepackage{graphicx}`
        
        It should be placed along with the other `\usepackage` lines.
    
    4.  Within your document (after `\maketitle` and before `\end{document}`)
        add the lines
        
        ```
        \begin{center}
        \includegraphics[width=0.75\textwidth]{name of your graphic file}
        \end{center}
        ```
        
        Change `name of your graphic file` to the filename of the graphic you want to include.
        This should not include the filetype extension.
        For example, to include `hilarious_math_meme.jpg` we would write
        
        `includegraphics[width=0.75\textwidth]{hilarious_math_meme}`
    
    5.  View your PDF to make sure the graphic got included correctly.
        
    That's it.
    Please find or make an image you'd like to share and include it in your document.
    
    Additional notes:
    
    + The width may be adjusted as needed.
      The suggestion `0.75\textwidth` should be a reasonable default but you might have
      to shrink it if your image is very tall.
    
    + You might run into trouble if your graphic file has spaces in its filename.
      You might want to rename it to something without spaces, e.g.,
      rename `hilarious math meme.jpg` to `hilariousmathmeme.jpg`.
    
    + If you run into other problems,
      you might be able to find help online
      (search online for the error message you're getting)
      but you're also welcome to contact me for help.
      I'll be happy to help you!
    
    Once you know how to do that, you will be able to add more features
    such as cropping, placing multiple images together, adding captions to figures, etc.
    (See for example <https://www.overleaf.com/learn/latex/Inserting_Images>
    or the documentation of the `graphicx` package.)
    For this assignment we are focussing on the basic core of including an image.
    
    In the next assignment we will see how to *create* images and diagrams within LaTeX.
    
    
2.  **Proposition 10.8 parts (ii)-(iii)**
    
    This is asking you to prove some basic properties of the absolute value.
    Since the definition of the absolute value $$|x|$$ involves two cases ($$x \geq 0$$ or $$x < 0$$),
    your proofs will mostly involve checking different cases,
    dividing up over cases where $$x \geq 0$$ or $$x < 0$$, and likewise for $$y$$ in part (ii)
    (so you will have cases of combinations, like $$x \geq 0$$ and $$y < 0$$, and so on).
    
    *LaTeX*: Absolute values like $$|x|$$ can be typed with the `|` key which
    is on the same key as the backslash `\`, above the return/enter key, on most keyboards.


3.  **Proposition 10.8 part (v)**, plus the converse. Specifically:
    
    1.  Prove Proposition 10.8(v) the way it's stated in the textbook.
    
    2.  Is the converse true? The converse is:
        
        *If $$\lvert x\rvert < \lvert y\rvert$$ then $$-y < x < y$$.*
        
        Prove or give a counterexample.
    
    3.  Prove this modification of the converse:
        
        *Suppose $$y > 0$$. If $$\lvert x \rvert < \lvert y \rvert$$ then $$-y < x < y$$.*
    
    Hint: Consider cases depending on whether $$x \geq 0$$ or $$x < 0$$.


4.  **Proposition 10.10 parts (i)-(iii)**
    
    Hint: Try to use propositions from section 10.2 (Absolute Value) as much as possible.


##  Additional assignments, required

These items are assigned and required.
You do not have to turn in anything.
These items will not be graded.

+   Read Chapters 11-12 of the textbook.



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

+ Read about big numbers:
  
  + [Part 1: From 1 to 1,000,000](https://waitbutwhy.com/2014/11/from-1-to-1000000.html)
  
  + [Part 2: From 1,000,000 to Graham's Number](https://waitbutwhy.com/2014/11/1000000-grahams-number.html)
  
  (Warning: Some spicy language.)

