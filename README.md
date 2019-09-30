# Project mandex (man index)

As I increasingly depend on *man* files as references and
learning resources, there are times when I waste a lot of
time on unsuccessful searches, particularly for large *man* 
files like *bash*, *xterm*, *wget*, etc.

This small script reads the text of a *man* file to collect
the sections names, presenting the section names in a list,
with one of the sections highlighted.

The user can change the highlighted section name using the
up or down arrow keys, or with Ctrl-N and Ctrl-P for the
next and previous lines, respectively.  Pressing ENTER on
a section name will launch **man** at the indicated section
name.

The first version offers only first-level indexing.  First-level
indexing is not always helpful (see the **gcc** man page),
so second-level indexing is on the way.

## Revelations

As usual, part of my motivation for developing a tool is for
the exploration of obscure (to me) details of the Linux OS.

With this project I hope to begin a habit of creating a 
supplemental page with my questions and discoveries, to leave
bread crumb trails of knowledge I can find later exploit to
recall successes and revisit useful web resources.

[README_learning.md](README_learning.md)
