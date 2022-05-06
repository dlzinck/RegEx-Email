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

A quantifier is a cool little tool we can use to determine how many times a specific character or group of characters needs to be present in order to have a match. For example if we look at our code for matching the email:
```
([a-z0-9_\.-]+)
```
this is trying to match any string that contains a-z, 0-9, _, ., or -. The quantifier + means that it has to contain at least one of these in order to have a match!


### Grouping Constructs

So let's talk about grouping constructs. Our first group that is in our email regex is:
```
([a-z0-9_\.-]+)
```
So this is the first group that appears in our regex. This must be true before moving on to "match" the next part of the code.
```
([\da-z\.-]+)
```
That was our second group that appears in this email regex.
```
([a-z\.]{2,6})
```
Last but not least, that was our third and final group that appears in this email regex.
In order to move on we have to make sure we are following the guidelines of the group before moving on to the next group. That’s just how it works!


### Bracket Expressions

In this part we will be looking at one group of symbols in depth, the all powerful brackets!
```
[ ] { } ( )
```
Brackets [ ] indicate a set of characters to match. Any individual character between the brackets will match, and you can also use a hyphen to define a set!
Curly braces { } are used to specify an exact amount of things to match. They are used after an expression and will only match 'na' exactly twice!
Parentheses ( ) represent remembered matches. This is especially useful for find-and-replace operations or any time you need to do something with only part of the match.

There are many ways to use bracket expressions and I encourage you to try and understand their concepts! 


### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)