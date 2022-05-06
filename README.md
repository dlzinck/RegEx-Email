# RegEx-Email

This is a tutorial and walk through on what a regular expression is and one of the ways to use them. Regular Expressions otherwise known as RegEx can be used when you are trying to match a certain character combination within a string. This is great for pulling out information from a given body of code as well as being used for validation. For example, this tutorial will follow an example code snippet that can be used to match an email. This tutorial will follow the different components that regular expressions have.


## Summary

The code following this summary will be used throughout the tutorial to give examples for how the components of regex can be used and how this particular code is used to match an email. So in other words with this code you will be able to validate an email to make sure it follows the proper format!

```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```


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

### Anchors

An anchor is what starts and ends the regular expression.
```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
So in this code snippet the anchors are ^ and $

This code snippet is looking for information that starts with
```
^([a-z0-9_\.-]+)
```
and ends with
```
.([a-z\.]{2,6})$
```
So what does the anchor mean? Well if we are to find a match it has to follow those initial guidelines. So, it must start and end with the given parameters within the code. If it does not, then it isn’t a match for us!


### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)