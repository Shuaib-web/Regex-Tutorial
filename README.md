# Regex Expressions Tutorial

Regular expressions are patterns used to match character combinations in strings. In JavaScript, regular expressions are also objects. These patterns are used with the exec() and test() methods of RegExp, and with the match(), matchAll(), replace(), replaceAll(), search(), and split() methods of String. 

## Summary

A regular expression is a pattern that is matched against a subject string from left to right. Regular expressions are used to replace text within a string, validate forms, extract a substring from a string based on a pattern match, and so much more. Regex is a case-sensitive language. The criteria must be strict when you use it to match the words. Below is the example to be illustraed in this tutorial

Example:

/^([a-z0-9_\.-]+) @([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Character Classes](#character-classes)

## Regex Components

### Anchors

Anchors, or atomic zero-width assertions, specify a position in the string where a match must occur. When you use an anchor in your search expression, the regular expression engine does not advance through the string or consume characters; it looks for a match in the specified position only. For example, ^ specifies that the match must start at the beginning of a line or string. Therefore, the regular expression ^http: matches "http:" only when it occurs at the beginning of a line.

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. 

### Grouping Constructs

Grouping constructs delineate the subexpressions of a regular expression and capture the substrings of an input string. You can use grouping constructs to do the following:

Match a subexpression that is repeated in the input string.

Apply a quantifier to a subexpression that has multiple regular expression language elements.

### Character Classes

A character class defines a set of characters, any one of which can occur in an input string for a match to succeed the regular expression language in 

## Author

My name is Shuib Mohamed and im currently studying to become a full stack developer. My link for the GitHub Gist is as follows:
