# Zip Code Regex Tutorial

## Summary

I chose to describe a regex that accepts American zip codes.
This expression accepts either 5-digit strings or 5-digit strings followed by a hyphen and a 4-digit string.

\d{5}(-\d{4})?

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
The parentheses in this expression act as a grouping construct to separate the hyphen and 4-digit group from the rest of the expression.

### Bracket Expressions
This expression does not use a bracket expression.
Bracket expressions are used to match exact characters or ranges of characters. To exclude characters, a caret can be placed ahead of the negated set of characters.

### Character Classes
In this expression, \d is a short-hand for a character class that signifies digits between 0 and 9.

### The OR Operator
This expression does not use an OR operator, but the optional second group works similarly. To write this expression with an OR operator, it would be \d{5}|\d{5}-\d{4}.

### Flags
This expression does not contain any flags, but they can be placed after a delimiter. Common flags are g and m. g signifies global, meaning it will match as many times as needed within the input string. m signifies multi-line, which affects anchors to match with the beginning and ending of lines within a string and not just the string itself.

### Character Escapes
This expression uses a character escape of \d. The backslash here lets the character d escape its direct meaning so that it now signifies digits between 0 and 9.

## Author
github.com/DaniSweets