Archlinux ABS Git
=================

This is a unofficial mirror of the Archlinux svn server.

Why
---------------

I maintain alot of my own packages and tracking changes 
using just abs was not enough and svn did not keep the 
same abs structrue and provided no logging.. among other things.

How it works
---------------

Once a day I run git svn fetch and pull any changes into the svn branch.
The svn branch contains the exact untouched archlinux svn it also contains
the same svn commit logs. 

I then rebase the svn branch into master. Master has been layed out to represent
abs. The layout only needed to be done once and rebasing takes care of the rest. 

Issues
--------------

If you have any issues with the master branch vs the svn branch . please post an
issue @ [Issues](http://github.com/str1ngs/abs/issues)

The master branch is still not stable enough to replace abs. However if you 
are in doubt you can use the svn branch it remains untouched. 

There are some problems when new packages are moved around in svn. Right now I have
a script that detrunks where needed but I think git can handle it alone if you are
git savy maybe you can take a look at it.

The mirror does not contain the full archlinux svn history its only contains
from revision 84267 on. I do not plan on pulling that history.

The svn commits are kinda cryptic. I need to dig deeper and find a better way to present them.

How to Contribute and use it
--------------

Contributing is very easy start by _watching_ the project on github. From there on you can
pull from this repo. Please try not to fork the project watching and cloning this repo should 
be enough.
