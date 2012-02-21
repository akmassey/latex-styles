# Aaron Massey's LaTeX Styles #

This repository contains various LaTeX style files I created with example source files that demonstrate their use.  Most of these are basic extensions to the [todonotes package][1].  Some of them are just my preferences for personal use.


## The Privacy Place ## 

File: tpp.sty

These styles replicate the style of the MS Word comments, but hard code the authors and colors.

#### Usage ####

Each author has their own command defined in the style file.  Currently, there are commands for Aaron, Pat, Annie, and Jessica.  To create a comment simply use the command in the LaTeX file as the following examples demonstrate.

You can create a comment that points to a highlighted section of text:

    Lorem ipsum dolor sit amet, \akm[This is comment text.]{This is text to be highlighted in the document.}consectetur adipisicing elit. 

You can also create a comment that simply points to the location where you inserted it in the text:

    Lorem ipsum dolor sit amet, \akm[This is comment text.]consectetur adipisicing elit. 

Please see the `simple-tpp-example.tex` file for more examples.

Please note that comments will only appear if the document is in draft mode:

    \documentclass[draft]{article}

If you remove the `draft` declaration, then the comments will not be generated and any text that would have been highlighted will appear as normal text in the document.


## Personal Preferences ##

File: akmassey.sty

These are personal preferences and styles that I use whenever I can.  You may find something interesting there.


## MS Word Style Comments ##

File: msword.sty

This package is still very much a work in progress.  It is intended to mimic most of the commenting functionality found in Microsoft Word.  Eventually, I would like to use this to replace the current tpp.sty file, but it's just not ready yet.  If you are interested in helping me get this working, please see the `akmassey-style-test.tex` file. 

[1]: http://www.ctan.org/tex-archive/macros/latex/contrib/todonotes/