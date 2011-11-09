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

The various options are
*   indent\_size \(default 4\) - how far to indent
*   indent\_char \(default space\) - the character to use for indentation
*   preserve\_newlines \(default true\) - whether or not line breaks should be kept
*   preserve\_max\_newlines (default unlimited) - maximal number of line breaks in a row to be preserved
*   jslint\_happy \(default false\) - jslint options
*   brace\_style \(default collapse\) - where to put opening braces.  This can be:
    *   collapse - braces go on the same line as the statement
    *   expand - braces go on their own line
    *   end-expand - just end braces go on their own line
