# Hex RegEx Tutorial

Hexadecimal is a number system that uses 16 different instances of symbols. These characters include 0-9 and both A-F (uppercase) and a-f (lowercase).

## Summary

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

Above is the regEx I'm going to explain. First, I'll explain RegEx itself. RegEx is a combination of characters that is used primarily to represent colors in RGB values.
Regular Expressions are a combination of characters that shows search patterns in regards to text. Characters can be both literal or meta, using their respective anchors.
Meta characters are representations of larger character sets.

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
RegEx Anchors include `^` and `$`.

The `^` marks the beginning of a line or string. The `$` symbol represents the end. So, '^ssbm' would match any item starting with SSBM. SSBM$ would match items that end with SSBM.

Hex RegEx is done front to back, so both are used.


### Quantifiers

Quantifiers set limits of strings your RegEx matches. They normally include both minimum and maximum characters per regex.
Quantifiers match every occurrence of the pattern that you define. 
`?` - Matches either once or not at all
`{}` - Has three different definitions for match number. {x} means exactly x number of times, {x,} matches at least x number of times, and { n, x }matches between n and x number of times.

You can also add a ? symbol to have your regEx search for the fewest possible combinations. 


### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
