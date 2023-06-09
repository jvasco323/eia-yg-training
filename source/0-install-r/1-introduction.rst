Installing R
============

**Robert J. Hijmans**, UC-Davis

--------------

**Background R software**
-------------------------

*R* is perhaps the most powerful computer environment for data analysis
that is currently available. *R* is both a computer *language*, that
allows you to write instructions, and a *program* that responds to these
instructions. *R* has core functionality to read and write files,
manipulate and summarize data, run statistical tests and models, make
fancy plots, and many more things like that. This core functionality is
extended by hundreds of packages (plug-ins). Some of these packages
provide more advanced generic functionality, others provide cutting-edge
methods that are only used in highly specialized analysis.

Because of its versatility, *R* has become very popular across data
analysts in many fields, from agronomy to bioinformatics, ecology,
finance, geography, pharmacology and psychology. You can read about it
in this article in
`Nature <http://www.nature.com/news/programming-tools-adventures-with-r-1.16609>`__
or in the `New York
Times <http://www.nytimes.com/2009/01/07/technology/business-computing/07program.html?pagewanted=all&_r=0>`__.
So you probably should learn *R* if you want to be good in data
analysis, be a successful researcher, collaborate, get a `high
paying <http://www.sfgate.com/technology/businessinsider/article/10-Tech-Skills-That-Will-Earn-You-Over-100-000-5193599.php>`__
data science job, … If you are not that much into *data analysis and
visualization* but want to learn programming for more general tasks, you
may want to start with `python <https://docs.python.org/2/tutorial/>`__
instead.

This document provides a concise introduction to *R*. It emphasizes what
you need to know to be able to use the language in any context. There is
no fancy statistical analysis here. We just present the basics of the
*R* language itself. We do not assume that you have done any computer
programming before (and if that is the case, we do assume that you think
it is about time you did). Experienced *R* users obviously need not read
this. However, the material may be useful if you want to refresh your
memory, if you have not used *R* much, or if you feel confused.

When using this resource, it is very important to follow `Norman
Matloff <https://www.nostarch.com/artofr.htm>`__\ ’s advice: *“When in
doubt, try it out!”*. That is, test yourself. Copy the examples shown,
and then make modifications to see if you can predict what will happen.
Only then will you really understand what is going on. You are learning
a language, and you will have to use it a lot to become good at it. So
express yourself and accept that for a while you will be stumbling a lot
and sometimes feel lost.

To work with *R* on your own computer, you need to
`download <https://cran.r-project.org/>`__ the program and install it. I
recommend that you also install `R-Studio <https://www.rstudio.com/>`__.
R-Studio is a separate program that makes *R* easier to use. Here is a
`video <https://www.youtube.com/watch?v=FIrsOBy5k58>`__ that shows how
to work in R-Studio.

After having gone through the chapters presented here, you should could
consult additional resources to learn *R*. It is very helpful to read
several of these introductions to *R* while you use it in your work.
Each time you will pick up new things, and feel accomplished about how
much you already understand. There are many free resources on the web,
including `R for
Beginners <http://cran.r-project.org/doc/contrib/Paradis-rdebuts_en.pdf>`__
by Emmanuel Paradis and this
`tutorial <http://www.cyclismo.org/tutorial/R/>`__ by Kelly Black that
is similar to the one you are reading now. Or consult this `brief
overview <https://www.stat.auckland.ac.nz/~ihaka/120/Notes/ch02.pdf>`__
by Ross Ihaka (one of the originators of R) from his `Information
Visualization <https://www.stat.auckland.ac.nz/~ihaka/120/notes.html>`__
course. You can also consult the more formal “official”
`introduction <https://cran.r-project.org/doc/manuals/r-release/R-intro.pdf>`__
or get a copy of Norman Matloff’s book `The Art of R
Programming <http://www.nostarch.com/artofr.htm>`__.

There is also a lot of good stuff on
`rstatistics.net <http://rstatistics.net/>`__

If you want to take it easy, or perhaps learn about R while you commute
on a packed train, you could watch some `Google Developers
videos <http://www.youtube.com/playlist?list=PLOU2XLYxmsIK9qQfztXeybpHvru-TrqAP>`__.

If none of this appeals to you, and you already are experienced with
*R*, or you have done a lot of programming with other languages, skip
all of this and perhaps have a look at Hadley Wickham’s `Advanced
R <http://adv-r.had.co.nz/>`__.

--------------

**Installing R on Windows**
---------------------------

`Download <https://cran.r-project.org/bin/windows/base/>`__ the latest R
installer (.exe) for Windows. Install the downloaded file as any other
windows app.

--------------

**Installing Rstudio on Windows**
---------------------------------

Now that R is installed, you need to download and install RStudio. First
`download <https://www.rstudio.com/products/rstudio/download/#download>`__
the installer for Windows. Run the installer (.exe file) and follow the
instructions.
