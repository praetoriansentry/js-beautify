Node JS Beautifier
---------------


This is the same beautifier as from [jsbeautifier.org](http://jsbeautifier.org/).  I've just taken the
JS and made it so it can be more easily excuted from the commandline on
systems with node.

I wouldn't be surprised if there is something that already does this, but
I couldn't find it fast enough.

Here are some example uses

    ./beautify.js file.js > out.js
    ./beautify.js --jslint_happy=true file.js > out.js
    ./beautify.js --indent_size=8 --jslint_happy=true file.js > out.js
    ./beautify.js --indent_char="\t" --indent_size=1  file.js > out.js

The various options are:

 *   `indent_size` \(default 4\) - how far to indent
 *   `indent_char` \(default space\) - the character to use for indentation
 *   `preserve_newlines` \(default true\) - whether or not line breaks should be kept
 *   `preserve_max_newlines` (default unlimited) - maximal number of line breaks in a row to be preserved
 *   `jslint_happy` \(default false\) - jslint options
 *   `brace_style` \(default collapse\) - where to put opening braces.  This can be:
    *   `collapse` - braces go on the same line as the statement
    *   `expand` - braces go on their own line
    *   `end-expand` - just end braces go on their own line
