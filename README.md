# REGEX Tutorial

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

Anchors match a specific location such as the beginning or end of a line or word.

There are two types of anchors in regex:

The caret (^) anchor  matches the beginning of a line or string. For example, the regex pattern "^monash" would match any string that starts with "monash".

The dollar sign $ anchor matches the end of a line or string. For example, the regex pattern "univeristy$" would match any string that ends with "university".


### Quantifiers

Quantifiers are used to specify how many times a character, group, or character class should be matched in a given string.

For example,

The asterisk () quantifier matches zero or more occurrences of the preceding character or group. For example, the regex pattern "ab" would match "a", "ab", "abb", "abbb", and so on.


### OR Operator

The OR operator is denoted by the symbol "|". It allows you to match one pattern or another.

For example, the Regex pattern "Monash|University" will match either "Monash" or "University". 

### Character Classes

Character class is a set of characters that you want to match. Character classes make it easy to match any character that belongs to a specific group or category, such as all digits or all whitespace characters.

\d - Matches any digit (0-9).
\D - Matches any character that is not a digit.
\w - Matches any word character .
\W - Matches any character that is not a word character.
\s - Matches any whitespace character .
\S - Matches any character that is not a whitespace character.

### Flags

There are 6 type of flags in Javascript,

i: The i flag makes the matching case-insensitive, meaning that uppercase and lowercase characters are treated as equivalent. For example, /Monash/i would match "Monash", "MONASH", and "monash".

g: The g flag enables global matching, which means that the pattern will match all occurrences in the input string rather than just the first one. For example, /a/g would match all occurrences of the letter "a" in the input string.

m: The m flag enables multi-line matching, which allows the pattern to match at the beginning or end of each line in a multi-line input string. For example, /^monash/m would match the word "monash" at the beginning of each line.

s: The s flag enables "dotall" mode, which allows the . metacharacter to match any character, including newline characters. 

u: The u flag enables Unicode matching, which allows the pattern to match Unicode characters beyond the ASCII range.

y: The y flag enables "sticky" matching, which means that the pattern will only match at the current position in the input string. 

### Grouping and Capturing

Grouping and capturing are techniques used to match and extract specific parts of a pattern.

Grouping is the process of enclosing part of a regex pattern in parentheses (). This is typically used to apply a quantifier, such as *, +, or ?, to a group of characters or subpatterns. For example, the pattern (ab)+ matches one or more occurrences of the sequence "ab" in a string.

Capturing is the process of using parentheses () to define a subpattern within a regex pattern, and then using that subpattern to extract specific text from the matched string. Each set of parentheses creates a capturing group that can be accessed by its index or name. For example, the pattern (\d{3})-(\d{3}-\d{4}) captures a phone number in the format of "123-456-7890" and stores the area code and the rest of the number in separate capturing groups.

### Bracket Expressions


### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
