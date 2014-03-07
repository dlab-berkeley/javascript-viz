javascript-viz
==============

This is a repository taking ideas from @rdhyee's [2014 Working with Open Data
class](https://github.com/rdhyee/working-open-data-2014). We present the basics
of using Javascript to plot and map things, starting with IPython notebooks,
then graduating to understanding how you'd coordinate that on your own with a
server.

Using the IPython notebook
--------------------------

This course won't use much python. BUT, it turns out the IPython notebook is a
generally useful place to write all kinds of code. JavaScript can melt your
brain. IPython can cool it off.

We'll also use the python interpreter to lauch a SimpleHTTPServer, this will
provide us with a simple example of how we might work in a "real" networked
situation.

Learning Javascript
-------------------

There are many resources to learning javascript. The following is probably not
the best, but it (like the IPython notebook) provides an *executable* textbook:

[Eloquent Javascript (2nd ed.
preview)](http://eloquentjavascript.net/2nd_edition/preview/)

Terms
----

**JSON** stands for JavaScript Object Notation. It's not so hard to understand the
structure once you get used to it, and [this online
editor](http://www.jsoneditoronline.org/) can help you explore it while you're
getting started, and might even become a part of your toolbox!

JSON is used in all kinds of situations - often where folks may have
historically used XML. For example, the IPython Notebook files (.ipynb) are
stored in JSON format.

**SVG** XML format for vector graphics
**Vector Graphics** “Like Illustrator”

Rough Curriculum
----------------

 1. First pass at some D3
 2. Intro to some easier high-level libraries
   - Dimple.js (and friends)
   - How to spin up a server quickly from the command line
 3. Intro to mapping
 4. Good Architecture for mapping
 5. Using developer features of the browser

Some simple how-to's
--------------------

### To run a simple local webserver:

    python -m SimpleHTTPServer

Go inside the static directory before firing up the web server!

### CSS selectors

It'll be very useful to learn how to use CSS selectors, they are used to select
the portion of the HTML (and SVG) code that your JavaScript will operate on.
This is [a CSS selector tutorial for
novices](http://code.tutsplus.com/tutorials/the-30-css-selectors-you-must-memorize--net-16048)

### Accessing the VM as a server:

The VM for the class is set up to support SSH access over port 2222 and HTTP
access via port 8000 -- both on localhost / 127.0.0.1. For example, you can open
up a browser in your “host” OS and type `localhost:8000` into the web browser
navigation bar.

From command line (Terminal, Git Bash):

    ssh -p 2222 ct@localhost

Or you can use Putty, etc. and type the appropriate bits into the appropriate
fields. Contact me if you have trouble with this. If you're going to do serious
development on Windows, I *highly* recommend installing Git for Windows, and
using the Git Bash tool (if you have strange errors with Git Bash, downgrade to
the previous version).
