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

In our email regex we have:
```
\d
```
as our character class. It will match a single letter character from a-z after the @ sign in the email address. Ensuring that a letter is matched after the @ in the email and not a number or special character.


### The OR Operator

The OR operator otherwise known as Alteration is basically just “OR” for regex. It is denoted as a vertical line character ```|``` .
 
Unfortunately we do not have any in our example regex for emails so we won't be going over it but I encourage you to do your research too!


### Flags

You’re starting to see that regular expressions are powerful patterns that provide a way to search and replace. Regular expressions may have flags that affect the search and as of right now there are only 6 of them in JavaScript:
```
i
g
m
s
u
y
```
As you can see we don't have any flags in our example regex for emails so we won't be going into great detail but I once again encourage you use your GoogleFu!

### Character Escapes

Let’s say we want to find something like a dot. Not “any character”, but just a dot. To use a special character as a regular one, prepend it with a backslash like so:
```
\ .
```
That’s what we call “escaping a character”. It’s pretty simple right? 
 
Not all code has to be difficult and as time goes on you will begin to understand and easily remember concepts to make your life a little easier but always remember your greatest tool…
GoogleFu - The art of googling


## Author

I have created this walkthrough to help fellow junior developers as part of one the many Challenges given at the UA Fullstack bootcamp.

Drew Zinck II
[GitHub](https://github.com/dlzinck)
[LinkedIn](https://www.linkedin.com/in/drewzinckii/)
[Contact Me](mailto:drew.zshell@gmail.com)