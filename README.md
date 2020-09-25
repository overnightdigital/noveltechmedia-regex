# Regular Expression Modifiers: Option Flags
## 1 re.I
## Performs case-insensitive matching.
## 2 re.L
## Interprets words according to the current locale. 
## This interpretation affects the alphabetic group (\w and \W), as well as word boundary behavior(\b and \B).
## 3 re.M
## Makes $ match the end of a line (not just the end of the string) and makes ^ match the start of any line 
## (not just the start of the string).
## 4 re.S
## Makes a period (dot) match any character, including a newline.
## 5 re.U
## Interprets letters according to the Unicode character set. This flag affects the behavior of \w, \W, \b, \B.
## 6 re.X
## Permits "cuter" regular expression syntax. 
## It ignores whitespace (except inside a set [] or when escaped by a backslash) 
## and treats unescaped # as a comment marker.


Regular Expression Patterns
# 1 ^
# Matches beginning of line.
# 2 $
# Matches end of line.
# 3 .
# Matches any single character except newline. Using m option allows it to match newline as well.
# 4 [...]
# Matches any single character in brackets.
# 5 [^...]
# Matches any single character not in brackets
# 6 re*
# Matches 0 or more occurrences of preceding expression.
# 7 re+
# Matches 1 or more occurrence of preceding expression.
# 8 re?
# Matches 0 or 1 occurrence of preceding expression.
# 9 re{ n}
# Matches exactly n number of occurrences of preceding expression.
# 10 re{ n,}
# Matches n or more occurrences of preceding expression.
# 11 re{ n, m}
# Matches at least n and at most m occurrences of preceding expression.
# 12 a| b
# Matches either a or b.
# 13 (re)
# Groups regular expressions and remembers matched text.
# 14 (?imx)
# Temporarily toggles on i, m, or x options within a regular expression. If in parentheses, only that area is affected.
# 15 (?-imx)
# Temporarily toggles off i, m, or x options within a regular expression. If in parentheses, only that area is affected.
# 16 (?: re)
# Groups regular expressions without remembering matched text.
# 17 (?imx: re)
# Temporarily toggles on i, m, or x options within parentheses.
# 18 (?-imx: re)
# Temporarily toggles off i, m, or x options within parentheses.
# 19 (?#...)
# Comment.
# 20 (?= re)
# Specifies position using a pattern. Doesn't have a range.
# 21 (?! re)
# Specifies position using pattern negation. Doesn't have a range.
# 22 (?> re)
# Matches independent pattern without backtracking.
# 23 \w
# Matches word characters.
# 24 \W
# Matches nonword characters.
# 25 \s
# Matches whitespace. Equivalent to [\t\n\r\f].
# 26 \S
# Matches nonwhitespace.
# 27 \d
# Matches digits. Equivalent to [0-9].
# 28 \D
# Matches nondigits.
# 29 \A
# Matches beginning of string.
# 30 \Z
# Matches end of string. If a newline exists, it matches just before newline.
# 31 \z
# Matches end of string.
# 32 \G
# Matches point where last match finished.
# 33 \b
# Matches word boundaries when outside brackets. Matches backspace (0x08) when inside brackets.
# 34 \B
# Matches nonword boundaries.
# 35 \n, \t, etc.
# Matches newlines, carriage returns, tabs, etc.
# 36 \1...\9
# Matches nth grouped subexpression.
# 37 \10
# Matches nth grouped subexpression if it matched already. 
# Otherwise refers to the octal representation of a character code.
