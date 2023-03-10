# Regex-how-to

A Regular Expression (Regex), is a sequence of characters that defines a search pattern. The search pattern can be used to match strings, or to perform some manipulation of the strings. It is a very useful tool for processing and analyzing text data.

## Summary

In this tutorial I will explain the use of a Regex to match emails. The expression for that will be /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ . Not to be alarmed by all the characters and symbols, as I will be breaking it all down below.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

The first anchor includes is (^) which indicates the start of a string. While the second anchor is ($) which indicates the end of the string.

### Quantifiers

Quantifiers included in this Regex are (+) and { n, x } or in this case {2,6}. The (+) matches one or more occurrences of the preceding character, group, or character class. Using this will combine every part of the email together. The {2,6} will allow a match range of 2-6 characters for the character set of [a-z\.] Matches the pattern from a minimum of 2 number of times to a maximum of 6 number of times.

### Character Classes

The Character class in the expression is (/d), and it will match any single digit from 0-9.  

### Grouping and Capturing

The primary way you group a section of a regex is by using parentheses (). Each section within parentheses is known as a subexpression. The three captured groups in the expression are ([a-z0-9_\.-]+), ([\da-z\.-]+), and ([a-z\.]{2,6}). 

### Bracket Expressions

Anything inside a set of square brackets ([]) represents a range of characters that we want to match. Our Regex includes three uses of the square brackets, with the first being [a-z0-9_\.-]This part represents the username part of an email, and matches one or more characters that can be lower-case letters, digits, periods, underscores, or hyphens. The second set of square brackets [\da-z\.-] matches one or more characters that can be digits, lower-case letters, periods, or hyphens. It represents the name of the email server. The last set of brackets [a-z\.] matches any character a-z and the character ".". It represents the top-level domain (.com).

### Greedy and Lazy Match

Quantifiers are inherently greedy, meaning they match as many occurrences of particular patterns as possible. Each of these quantifiers can be made lazy by adding the ? symbol after it, meaning it will match as few occurrences as possible. The two quantifiers in our expression are (+) and {2,6}. 

## Author

Mariano Rojano
Github profile: https://github.com/mawiano
