# Tutorial: Matching an Email With regex

A common feature in any website is creating a user and signing them up with their email. This tutorial will help you ensure that a user is entering an input that is at least in the correct format of an email. 

## Summary

Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

For a quick example, lets use "user@host.com". The above regex first checks for a valid handle for the user, in this case, "user". Then it looks for the "@" symbol. Then it checks for another set of characters (host), a period, and third set of characters for the domain type (com). 

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

A regex is made up of a series of tokens. We will briefly go over the tokens used and their meaning below. Again, we are using `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` 

### Anchors
An anchor describes a location. It could be the end of a line, the beginning of a string, or something else. In our example regex, we have a few. 

^ refers to the start of a string

A dollar sign refers to the end of a string

In languages other than javascript, different characters are used to define these (\a and \z)



### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
