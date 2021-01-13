What is the prodigalverse?
--------------------------

An ever expanding opinionated package of R functions with the same
underlying philosophy of doing one thing at a time and one thing only
%&gt;% obviating burdensome overhead and steep learning curve of
understanding overall generalisations of operations %&gt;% turning one
into a prodigy of data analysis %&gt;% this should be of great benefit
to new practicioners of data mining and machine learning applications
%&gt;% data wranglers and other kinds of analyst should also find use in
this library %&gt;% we are aiming at an audience of analysts who are
looking for practical results and who are less concerned with the grand
concepts which are primarily of interest to researchers but not
necessarily for real world practioners

Writing and working the prodigal way
------------------------------------

All help and instructions for the prodigalverse utilise the magrittr
“%&gt;%” to highlight the connectivity of concepts passing one easily
into the other to clarify the steps and increase readability of the
documentation rather than relying on potentially confusing embedded
punctuation concepts of the older language such as “.”, “;”, “–” %&gt;%
we have however retained the comma because of its functional similarity
to “%&gt;%” but which is also different %&gt;% this pays hommage to
previously used language functional structures in cases where these
older punctuation structures retain their merit under the efficient new
paradigm of the prodigalverse %&gt;% we have mixed opinions about
uppercase letters

A grammar of prodigy
--------------------

we recommend thinking of your analyses in the prodigalverse as
‘prodigious’ and grammar should follow accordingly %&gt;%

verb = prodigise

adverb = prodigiously

noun = prodigy

adjective = prodigal

Installing other packages
-------------------------

We strongly recommend that when using the prodigalverse that users
install and load every library on CRAN %&gt;% although functions from
these libraries will not always be used and they are not dependencies of
the prodigalverse, we believe that it useful to have that functionality
available for analyses should the need arise without having to install
and load a package in the middle of an analysis

Phase 1: the C-series of functions
==================================

This incredibly useful series of functions were the first additions to
the prodigalverse and allow one to careful build a vector of data in
steps %&gt;% this close connection to the data means that the analyst
becomes deeply familiar with their data having actively inspected and
inputed all the values %&gt;% this has been implemented at present for
vectors up to length 10 only but we are currently looking for
collaborators to create functions to populate vectors up to length 10^6,
matrices of dimension 10^6 x 10^6 and to arrays of up to 10^6 dimensions
%&gt;% although it is conceivable that there are cases where one would
need larger data structures, we consider these special cases and we
would refer those analysts to base R functions for such peculiar
situations

    x <-5
    x<- c2(x, position2x=8) 
    x<- c3(x, position3x=17.86) 
    x

    ## [1]  5.00  8.00 17.86

It is clear to see from these examples how one can build a vector of
values %&gt;% the true power of the C-series of functions becomes
apparent if we string the functions together with the magrittr to build
up the vector %&gt;% which we will now call the pgvector

    require(magrittr)

    ## Loading required package: magrittr

    x <- 12
    full.vector<-
     x %>%
      
     c2(.,position2x=5) %>%
      
      c3(.,position3x=18) %>%
      
        c4(.,position4x=4.1) %>%
      
         c5(.,position5x=126.3) %>%
      
          c6(.,position6x=78) %>%
      
            c7(.,position7x=0.1) %>%
      
              c8(.,position8x=2) %>%
      
                c9(.,position9x=53) %>%
      
                  c10(.,position10x=51) %>%
     print

    ##  [1]  12.0   5.0  18.0   4.1 126.3  78.0   0.1   2.0  53.0  51.0

Future plans
------------

We are also currently developing a series of functions that can multiply
each element of a vector, matrix or array by a value %&gt;% this series
of functions may take some time to get up and running because in order
to keep it understandable and simple, we must develop a separate series
of functions for each kind of operation such as addition, subtraction,
multiplication, division, square root, cube root, fourth root, square,
cube, factorial etc %&gt;% when developed, we anticipate that the
simplicity of this set of functions will be a gateway into modern
results based analysts who are not making production level code but who
need to achieve specific aims

Looking for collaborators
=========================

We welcome contributors sharing our philosophy %&gt;% aside from the
areas mentioned above, we are seeking collaborators who could work on
developing functions for a beautiful plotting series of functions,
deconstructing data structures element by element and of course any
other kind of analysis the community might find useful

Contracting
-----------

We are willing to provide contract based help and analysis %&gt;% please
email us with a description of your help or analysis issue, preferably a
sample data set and we can provide you with a detailed evaluation of
what would be involved and a quote

<a href="mailto:prodigalverse@protonmail%" class="email">prodigalverse@protonmail%</a>&gt;%com

You are welcome and we wish you prodigious code and analysis!
