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

## TruffulaOptions.java / TruffulaOptionsTest.java
the actual configs. passed in from app.java.
primarily a handler to ensure we're passed valid arguments.
handles the root directory, if hidden files are shown, or if colorprinter actually does color.
tests should probably get expanded to: make sure all args get set by default. intentionally wrong values for color/hidden files is handled. right values are handled.

## TruffulaPrinter.java / TruffulaPrinterTest.java

## AlphabeticalFileSorter.java