# Regex-how-to

A Regular Expression (Regex), is a sequence of characters that defines a search pattern. The search pattern can be used to match strings, or to perform some manipulation of the strings. It is a very useful tool for processing and analyzing text data.

## Summary
In this tutorial I will explain the use of a Regex to match emails. The expression for that will be /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ . Not to be alarmed by all the characters and symbols, as I will be breaking it all down below. 


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
The first anchor includes is (^) which indicates the start of a string. While the second anchor is ($) which indicates the end of the string.

### Quantifiers
Quantifiers included in this Regex are (+) and {2,6}. The (+) matches one or more occurrences of the preceding character, group, or character class. Using this will combine every part of the email together. The {2,6} will allow a match range of 2-6 characters for the character set of [a-z\.] Matches the pattern from a minimum of 2 number of times to a maximum of 6 number of times.

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions
Anything inside a set of square brackets ([]) represents a range of characters that we want to match. Our Regex includes three uses of the square brackets, with the first being [a-z0-9_\.-]This part represents the username part of an email, and matches one or more characters that can be lower-case letters, digits, periods, underscores, or hyphens. The second set of square brackets [\da-z\.-] matches one or more characters that can be digits, lower-case letters, periods, or hyphens. It represents the name of the email server. The last set of brackets [a-z\.] matches any character a-z and the character ".". It represents the top-level domain (.com). 

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

Mariano Rojano 
Github profile: https://github.com/mawiano 
