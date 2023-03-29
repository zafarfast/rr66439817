# REGEX Tutorial

REGEX Tutorial for beginners

## Summary

Regular expressions, commonly known as "regex," are a powerful tool used to search, manipulate, and extract text data. This tutorial aims to provide a comprehensive introduction to regex, covering the basics of syntax and operators.

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
A bracket expression (also known as a character class) is a way to match any single character from a set of characters. Bracket expressions are enclosed in square brackets [], and can contain a list of characters, ranges of characters, or a combination of both.

For example, the pattern [xyz] matches any single character that is either "x", "y", or "z". The pattern [a-z] matches any single lowercase letter from "a" to "z", while the pattern [A-Z0-9] matches any single uppercase letter or digit.

### Greedy and Lazy Match

Greedy and lazy matching are two ways to control how the pattern matching engine handles repeated patterns.

Greedy matching is the default behavior, where the engine tries to match as many characters as possible while still satisfying the pattern. This means that a greedy quantifier, such as *, +, or {n,}, will match as many repetitions as possible before moving on to the next part of the pattern. For example, the pattern a.* b would match the entire string "afoo bar baz bqux" because the .* quantifier greedily matches all characters between the "a" and the "b".

Lazy matching, on the other hand, matches as few characters as possible while still satisfying the pattern. This is achieved by adding a question mark ? after the greedy quantifier. For example, the pattern a.* ?b would match only the substring "ab" in the same string "afoo bar baz bqux".


### Boundaries

Boundaries are used to match specific positions within a string or text. They are not actual characters, but rather, they are assertions or conditions that define the start or end of a word, line, or string.

There are different types of boundaries in regex, including:

Start of Line (^): Matches the beginning of a line or string.

End of Line ($): Matches the end of a line or string.

Word Boundary (\b): Matches the position between a word character (any letter, digit, or underscore) and a non-word character (any character that is not a letter, digit, or underscore).

Non-Word Boundary (\B): Matches the position that is not between a word character and a non-word character.

Start of Word (\B): Matches the position that is not the start of a word.

End of Word (\B): Matches the position that is not the end of a word.


### Back-references

Back-references are a way to reference previously captured groups within the same pattern. When creating a regex pattern, you can use parentheses to create a capturing group, which will store the matched text for later use. 

To use a back-reference, you simply need to include the number of the capturing group inside a backslash followed by that number. For example, if you have a capturing group that matches a string of digits, you could use a back-reference to match that same string of digits again later in the pattern.


### Look-ahead and Look-behind


## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
