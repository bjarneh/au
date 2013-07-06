
    au - guess encoding and convert it to utf-8


## What ##

`au` guesses file encoding and converts it to [UTF-8][3].
Guessing is not done using [chardet][4] since that tool
cannot distinct between [ISO-8859-1][6] and [ISO-8859-2][5]
very well, i.e. it does not work well for Norwegian.
Instead the guessing is copied from the standard Unix [file][1]
tool, which is speedy and works great for Norwegian.


## Requirements ##

- [Python][2]


## Try it ##

The script itself can be found inside the `bin` folder, i.e.
either copy it from there to your `PATH` or add that directory
to your path to run the program.

    $ git clone https://github.com/bjarneh/au
    $ export PATH=$PATH:$PWD/au/bin
    $ au -r au/

And you should see some guess work being done.

[1]: https://github.com/glensc/file "File Github Repo"
[2]: http://python.org "Python Official Website"
[3]: http://en.wikipedia.org/wiki/UTF-8 "Wikipedia UTF-8 Page"
[4]: http://pypi.python.org/pypi/chardet "Python Chardet Package"
[5]: http://en.wikipedia.org/wiki/ISO/IEC_8859-2 "ISO-8859-2 Wikipedia Page"
[6]: http://en.wikipedia.org/wiki/ISO/IEC_8859-1 "ISO-8859-1 Wikipedia Page"
