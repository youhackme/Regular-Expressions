# Regular-Expressions
My journey to learn Regular Expressions


1. Symbol `.+`, the dot means any character and the `+` means one or more.
2. `^` match anything that is not a something e.g a space. E.g [^ ]
3. `?`, for the preceding character, that's optional e.g https?://
4. `?:` this is a none capturig group e.g `/idiot(?:ic)?/`
5. `*`: match zero or more
6. `.` : A period represents any character
7. `\w`: match a word.
8. `\t`: match a tab
9. `\s`: match a space character





Example:
This website is stupid. Your speaking style is idiotic. Your knowledge is crap. This is so stupid. You're an idiot.

Regex:
/stupid|idiot(?:ic)?|crap/g

Example:


Note: If you want to capture/extract match, wrap it into `()` and then access it using `$1`

Positive Lookaheads

1. `/google(?=<)/ig` matches <a href="http://google.com">`Google`</a>

Negative lookaheads:

1. `/google(?!<)/ig` matches <a href="http://google`.com">`Google`</a>`

Positive lookbehinds:

1. `/google(?<=)/ig` matches <a href="http://google.com">`Google`</a>
