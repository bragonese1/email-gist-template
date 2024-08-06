# E-MAIL REGEX

In this tutorial, I am going to cover the email address validation process using a regex pattern. Regex is short for the words "regular experssion". "Regular Expression" is a sequence of patterns that are used for string matching.  

## Summary

The regex pattern for email validation is as follows:
<br>

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

<br>

These symbols are a pattern that are designed to check if a string is a valid email. Though these symbols seem like that are a little random if you break it down it almost starts to resemble an email address.
<br>
<br>
Here is a breakdown of the symbols used in the regex pattern using the example email "fullstack@gmail.com":
<br>
- ([a-z0-9_\.-]+) = "fullstack" portion of the email
<br>
- @([\da-z\.-]+) = "@gmail" portion (as you can see the '@')
<br>
- .([a-z\.]{2,6}) = ".com" (as you can see it starts with the '.')
<br>

Further breakdown can be found below.


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
Anchors are like the start and end markers of a string.
<br>
- ^ = the caret is the start of the string
- $ = the dollar sign is the end of the string

These start and end markers make sure that the entire string is validated and not just a part of it.

### Quantifiers
Quantifiers function is similar to what it sounds like. It is like the counter of the regex. It gives a count of how many time the regex pattern should continue.
<br>
- `+` is similar to addition and is adding one or more to the previous.
<br>

For Example, in our previous example fullstack@gmail.com. The section `([a-z0-9_\.-]+)` that equalled the "fullstack" portion of our example email, ends with a `+`. This makes sures that the email before the `@` can have one or more of the characrters that are contained in the parenthesis.
### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)