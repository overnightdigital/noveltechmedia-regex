# Regular Expression Modifiers: Option Flags
## re.I
Performs case-insensitive matching.
## re.L
Interprets words according to the current locale. 
This interpretation affects the alphabetic group (\w and \W), as well as word boundary behavior(\b and \B).
## re.M
Makes $ match the end of a line (not just the end of the string) and makes ^ match the start of any line 
(not just the start of the string).
## re.S
Makes a period (dot) match any character, including a newline.
## re.U
Interprets letters according to the Unicode character set. This flag affects the behavior of \w, \W, \b, \B.
## re.X
Permits "cuter" regular expression syntax. 
It ignores whitespace (except inside a set [] or when escaped by a backslash) 
and treats unescaped # as a comment marker.




# Regular Expression Patterns
## ^
Matches beginning of line.
## $
Matches end of line.
## .
Matches any single character except newline. Using m option allows it to match newline as well.
## [...]
Matches any single character in brackets.
## [^...]
Matches any single character not in brackets
## re*
Matches 0 or more occurrences of preceding expression.
## re+
Matches 1 or more occurrence of preceding expression.
## re?
Matches 0 or 1 occurrence of preceding expression.
## re{ n}
Matches exactly n number of occurrences of preceding expression.
## re{ n,}
Matches n or more occurrences of preceding expression.
## re{ n, m}
Matches at least n and at most m occurrences of preceding expression.
## a| b
Matches either a or b.
## (re)
Groups regular expressions and remembers matched text.
## (?imx)
Temporarily toggles on i, m, or x options within a regular expression. If in parentheses, only that area is affected.
## (?-imx)
Temporarily toggles off i, m, or x options within a regular expression. If in parentheses, only that area is affected.
## (?: re)
Groups regular expressions without remembering matched text.
## (?imx: re)
Temporarily toggles on i, m, or x options within parentheses.
## (?-imx: re)
Temporarily toggles off i, m, or x options within parentheses.
## (?#...)
Comment.
## (?= re)
Specifies position using a pattern. Doesn't have a range.
## (?! re)
Specifies position using pattern negation. Doesn't have a range.
## (?> re)
Matches independent pattern without backtracking.
## \w
Matches word characters.
## \W
Matches nonword characters.
## \s
Matches whitespace. Equivalent to [\t\n\r\f].
## \S
Matches nonwhitespace.
## \d
Matches digits. Equivalent to [0-9].
## \D
Matches nondigits.
## \A
Matches beginning of string.
## \Z
Matches end of string. If a newline exists, it matches just before newline.
## \z
Matches end of string.
## \G
Matches point where last match finished.
## \b
Matches word boundaries when outside brackets. Matches backspace (0x08) when inside brackets.
## \B
Matches nonword boundaries.
## \n, \t, etc.
Matches newlines, carriage returns, tabs, etc.
## \1...\9
Matches nth grouped subexpression.
## \10
Matches nth grouped subexpression if it matched already. 
Otherwise refers to the octal representation of a character code.
