# Project mandex (man index)

The small script reads the text of a *man* file to
collect the section names, presenting the names in
a scrolling list from which a user can select and be
brought to that section of the man file.

## Man Details

**man** opens a man file and sends the contents to a
pager program.  By default on most systems, the pager
is **less**.

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