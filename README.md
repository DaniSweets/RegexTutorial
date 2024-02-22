# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

I chose to describe a regex that accepts American zip codes. \d{5}(-\d{4})?

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components
The components of this expression are 
 - \d
    This signifies any digit from 0 to 9.
 - {}
    This is a quantifier that tells us how many digits are in a row.
 - ()
    This separates a specific part of the expression from the rest.
 - ?
    This signifies that whatever is written directly beforehand (the parentheses in this case) can either happen or not, and still be valid.

### Anchors
This expression does not include anchors. The zip code can be found in any place within a string for it to be accepted.
If you'd like to only accept zip codes at the beginning or end of a string, you could add a ^ or $ to the expression.

### Quantifiers
This expression includes two quantifiers. These look for 5 digits in a row, and 4 digits in a row. These are shown with {5} and {4}.

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)