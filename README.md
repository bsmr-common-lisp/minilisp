MINIEXP/MINILISP
----------------

Files <miniexp.h> and <miniexp.cpp> in directory
<djvulibre-3.5/libdjvu/miniexp.h> implement the basic data
structure of a lisp interpreter: s-expressions.

S-expressions can be viewed as a simple and powerful
alternative to XML.  They are used in DjVu to handle
annotations.  Both the decoding api <ddjvuapi.h> and program
<djvused> use s-expressions to describe the hidden text
information and the navigation information (bookmarks.)

Comments in file <miniexp.h> describe which s-expressions
are supported, how they are represented in text files, and
which functions are available to handle them.


During the development of <miniexp.h> and <miniexp.cpp> it
appeared that the best way to test s-expressions was to make
the last step and program a complete lisp interpreter.  
This also makes a perfect example of using <miniexp.h>.

The core interpreter is in file <minilisp.cpp>.
Startup definitions are in file <minilisp.in>.
Just type <make> to compile it.

Exercise: speed up the interpreter by
accelerating the function lookup().

- Leon Bottou, 
  September 2005

