Resaw-rs
========

A regular expression saw.


Concepts
========

Resaw allows you to take example lines like this:

    example This is an example line with data=5.

And apply a pattern like this:

    pattern                                   d+

... to automatically create regular expressions like this:

    ^This is an example line with data=(\d+)\.$

... to capture fields named like this

    fields thedata

... that you can associate with named event types:

    name example_line


In a more composed form, it looks like this:

    name example_line
    example This is an example line with data=5.
    pattern                                   d+
    fields                                    thedata

