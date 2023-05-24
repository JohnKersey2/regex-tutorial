# Tutorial: Matching an Email With regex

A common feature in any website is creating a user and signing them up with their email. This tutorial will help you ensure that a user is entering an input that is at least in the correct format of an email. 

## Summary

Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

For a quick example, lets use "user@host.com". The above regex first checks for a valid handle for the user, in this case, "user". Then it looks for the "@" symbol. Then it checks for another set of characters (host), a period, and third set of characters for the domain type (com). 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs and Bracket Expressions](#grouping-constructs-and-bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)

## Regex Components

A regex is made up of a series of tokens. We will briefly go over the tokens used and their meaning below. Again, we are using `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` 

### Anchors
An anchor describes a location. It could be the end of a line, the beginning of a string, or something else. In our example regex, we have a few. 

^ refers to the start of a string

A dollar sign refers to the end of a string

In languages other than javascript, different characters are used to define these (\a and \z)



### Quantifiers

Quantifiers refer to how many of a certain portion of our regex should be present. Ours has a simple "Quantity", as described by {2,6}. This states that the final portion of our code should be somewhere between 2 to 6 characters. 

### Grouping Constructs and Bracket Expressions

Grouping constructs breakdown the entirety of the string the regex is looking at into substrings. There are broken up by parenthesis or square brackets. Square brackets are meant to capture specific characters, whereas parenthesis captures groupings of characters (and can hold things like quantifiers)

([a-z0-9_\.-]+) is a grouping, with a bracket expression inside of it. The @ symbol in our expression does not sit in a bracket expression or a group. 

### Character Classes

Character classes simply distinguish what kinds of characters your regex is looking for. It could be letters, digits, special characters, or any combination thereof. 

In our example 

\d matches any digit. 

a-z0-9_\.-  matches all alphanumber characters, underscore, and dash.

The \. means it should ignore periods, as \ tells it to escape the character.

### The OR Operator

| defines the or operator. While not in our expression, it's helpful to know in other expressions it allows you to search for one of two things. A developer may decide to allow . or , before the top level domain as , is a common typo for .

### Flags

This regex doesn't use one of the six flags in javascript. A developer could use the "i" taget to make a search for the email case insensitive, if pulling email from a website. A developer may use "g" to look at all matches, as regex only returns the first. They may also add "u" to enable full unicode support.  

## Author

John Kersey is a junior web developer from Atlanta. Please visit my [github here](https://github.com/JohnKersey2)
