# E-MAIL REGEX FOR BEGINNERS

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
The (parenthesis) as shown in the example above are used throughout our email regex for character grouping. The parenthesis break down the email regex into username, domain name, and top level domain.
### Bracket Expressions
The [brackets] are used to define the classes of the characters that we want to match. We will use the username portion to illustrate what that means:
<br>

`[a-z0-9_\.-]` = the 'a-z' matches letters, '0-9' matches digits, `_\.-` matches an underscore, dot, or hyphen that is in the username of the email.

### Character Classes
Character classes are used to match a single character or can be used for shorthand. Lets use the domain name portion of our email example:
<br>
- `[\da-z\.-]` = the '\d' is a shorthand for digits.
- `[\da-z\.-]` = the '\.' is a shorthand for a period.

### The OR Operator
The OR operator or "|" is not used in our email regex. But, it is used just like the name suggests. 1|2 would look to match 1 or 2.
### Flags
Flags are not used in our email regex either. These can be used to create optional rules that change how a regex behaves.
### Character Escapes
Character escapres are refering to the portion of our email regex that can be found in between the parenthesis of our domain and top domain and shown as `\.` which is representing a period or 'dot'. If the slash is not used then the dot would not be specifically looked for as a match.
## Author
Hello, I'm Bragonese1. I am a fullstack student who is still very much in the learning process and trying build a solid foundation of coding. This tutorial is not only written to aid myself, but also hopefully provide aid to other newbies. You can contact me at my [GitHub](https://github.com/bragonese1) and you can find this repo at this location [Github Repo](https://github.com/bragonese1/email-regex-beginners).