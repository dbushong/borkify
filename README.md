`borkify` is a small perl script that turns ASCII text into similar
looking but goofily chosen characters. Not very useful, though the
reverse mode (borkify -r) reverses the process... useful for getting
mostly useful ASCII out of accented "high-bit" text.

    % echo "This is really goofy." | borkify
    Ṯĥǐϟ îﺉ ṟêåļłỹ ǥŏõḟý∙

    % echo "Jöe Smíth uses “annoying smart quotes”" | borkify -r
    Joe Smith uses "annoying smart quotes"

It's also a node module that does the same:

```coffee
{ toASCII, fromASCII } = require 'borkify'

console.log toASCII 'Hérè ïs søme idiot’s text.'
# ==> Here is some idiot's text.

console.log fromASCII "Let's make this look really horrible."
# ==> ∟ẻţיš ḿăḵě †ḣ¡ﻱ ļỏőḵ ŗęǡłŀỹ ḧőŗṙíЫě∙
```
