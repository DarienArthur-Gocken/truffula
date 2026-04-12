# Truffula Notes
As part of Wave 0, please fill out notes for each of the below files. They are in the order I recommend you go through them. A few bullet points for each file is enough. You don't need to have a perfect understanding of everything, but you should work to gain an idea of how the project is structured and what you'll need to implement. Note that there are programming techniques used here that we have not covered in class! You will need to do some light research around things like enums and and `java.io.File`.

PLEASE MAKE FREQUENT COMMITS AS YOU FILL OUT THIS FILE.

## App.java
our main method / initial starting point.
will create the truffula options and fill them out based on args passed in.
has example of args.
truffulaoptions will be passed to truffulaprinter
and then we'll print truffula printer.

## ConsoleColor.java
handles standard ANSI color codes.
apply it in a string and it'll apply the color code that its set to.

## ColorPrinter.java / ColorPrinterTest.java
handles properly printing the text out, and handling consolecolor.
basically just a handler.
tests should probably get expanded to: pass in blank statements. verify you can print in the same color twice in a row w/o changing it.
if the colors look weird, look here.

## TruffulaOptions.java / TruffulaOptionsTest.java
the actual configs. passed in from app.java.
primarily a handler to ensure we're passed valid arguments.
handles the root directory, if hidden files are shown, or if colorprinter actually does color.
tests should probably get expanded to: make sure all args get set by default. intentionally wrong values for color/hidden files is handled. right values are handled.
if the options seem like they're getting weird, look here.

## TruffulaPrinter.java / TruffulaPrinterTest.java
pulls everything together.
this is what actually handles the recursion through files and folder structures.
if the folder structure printing looks weird, its probably this.
tests should be expanded to: test hidden vs non-hidden. test 1 folder no files. test 1 file in directory. test nothing in root.

## AlphabeticalFileSorter.java
sorts files alphabetically ignoring case.
will be used in wave 6 of truffulaprinter.