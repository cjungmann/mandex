# Project mandex Learning Page

[Main README](README.md)

## How MAN operates

The **man** command opens a man file and sends the contents
to a pager program.  By default on most systems, the pager
is **less**.

## Search MAN Using LESS Search Options

For this project, the **less** feature I am interested in
is how to position the output at a specific position in
the file.

There are at least two ways to do this, but the best of the
two is to set an environment variable, *LESS* to a search
string before calling **man**.  For example, to open the
**bash** man page at *Parameter Expansion*, issue the following
at the command line:

~~~sh
LESS=+/Parameter\ Expansion man bash
~~~

I recommend looking at the **less** man page to find other
features that you can exploit.

I hope this **mandex** utility will help make the study of
man pages easier.

## Idea for Future: LESS Bookmarks

There are two reasons bookmarks can be useful:

1. *To return where one left off.*  When reading a **man** to
   learn about a program or command, it would be nice to save
   one's place to continue reading later.

1. *To keep a list of helpful references.*  If a useful indexing
   schema can be developed, it would be nice to keep a list of
   user-labelled bookmarks into many available *man* pages.

## Testing with Long MAN Files

This is not earth-shatteringly useful, but here it is anyway.

Search for the longest *man* pages on your system with the
following command:

~~~sh
ls -S -l /usr/share/man/man1 | less
~~~

I searched for long *man* pages to see how **mandex** performs.
Trying different pages revealed problems that I neglected and
now plan to address.