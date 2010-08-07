`borkify` is a small perl script that turns ASCII text into similar
looking but goofily chosen characters. Not very useful, though the
reverse mode (borkify -r) reverses the process... useful for getting
mostly useful ASCII out of accented "high-bit" text.

    % echo "This is really goofy." | borkify
    Ṯĥǐϟ îﺉ ṟêåļłỹ ǥŏõḟý∙

    % echo "Jöe Smíth uses “annoying smart quotes”" | borkify -r
    Joe Smith uses "annoying smart quotes"
