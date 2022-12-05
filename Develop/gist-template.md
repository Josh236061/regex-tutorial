# REGEX Tutorial

Regex, or regular expressions, are collections of characters that produce text search patterns. Used most frequently in word processors, text editors, and search engines. You may find a thorough description of a specific regex, one that looks for hexadecimals, here. A letter-and-whole-number value scheme is used in hexadecimals. Hex can be difficult to find because they frequently start with a # and have different numbers of characters.

## Summary

The REGEX we will be discussing is a Matching Email expression. We will deconstruct this following statement : /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/.  

To ensure that a user inputs an email address that starts with an arbitrary amount of characters before the @ symbol, followed by a domain, each element of this regex has a specific duty.

We will identify the Anchors, Quantifiers,The OR Operator, Charecter Classes, Grouping and Capturing, Bracket expressions, Greedy and Lazy Match, Boundaries, Back-references, Flags and Look-ahead and Look-behind.

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
Anchors are used to “anchor” the regex match at a certain position. ^ matches the position before the first character in the string from the email, and $ matches right after the last character in the string.

### Quantifiers
Quantifiers indicate numbers of characters or expressions to match. {} is the quantifiers in this expression. {2,6} here means to check if the eamil domain .xx has 2 to 6 letters.

### OR Operator
OR Operator | indicates the logical "or". It doesn't have one here but you will use it in building a logical “or” operation using regular expressions.

### Character Classes
Character classes distinguish between various characters, such as letters and numbers. . usually comes with \, otherwise it repsents a wildcard character. \d is shorthand for digit 0 to 9.

### Flags
A flag is an optional parameter to a regex that modifies its behavior of searching. i (insensitive) makes the whole expression case-insensitive: no difference between A and a.

### Grouping and Capturing
Grouping and capturing () indicates groups of expression characters. ([a-z\.]{2,6}) here creates a capturing group with both [a-z\.] and {2,6}.

### Bracket Expressions
Bracket Expressions [] can match any values you put inside the []. [a-z0-9_\.-] here can match with charactersa-z, numbers0-9 or symbols _ . - that typically used in the email address.

### Greedy and Lazy Match
The quantifiers * + {} are greedy operators, so they expand the match as far as they can through the provided text. \da-z\.-]+ can match with any numbers, characters, and symbol. or -.

Lazy Match ? means to match the shortest possible string. By adding the ? after the * + {}, we tell it to repeat as few times as possible.

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
