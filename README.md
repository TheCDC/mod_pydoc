# prettypydoc
Attempt at modernizing the look of html pages served by pydoc

Pydoc is great - no, make that **fantastic**.
However, I (and apparently other people) do not like the choice of colors
for the pages served in a browser by pydoc.

The original pydoc module has hard-coded values for color choices.
This new version, based on html5, uses css styling.

To test with the default (fancy styling):

    prettypydoc.py -b

To use a user-defined css file:

    prettypydoc.py -b -c <path_relative_to_cwd>

For example, to see a css close approximation of the original css:

    prettypydoc.py -b -c classic

A more interesting example has been provided by u8y7541:

    prettypydoc.py -b -c custom.css

It looks like the following:

![screenshot](Screenshot01.png)
![screenshot](Screenshot02.png)

Finally, pydoc_test.css is included as an example of a very slightly
customized file (the background color is different from the new default).
To run it:

    prettypydoc.py -b -c pydoc_test.css
