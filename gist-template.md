# Hex RegEx Tutorial

    Hexadecimal is a number system that uses 16 different instances of symbols. These characters include 0-9 and both A-F (uppercase) and a-f (lowercase). Hex codes are normally used to correspond to colors  

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

## Anchors
    RegEx Anchors include `^` and `$`.

    The `^` marks the beginning of a line or string. The `$` symbol represents the end. So, '^ssbm' would match any item starting with SSBM. SSBM$ would match items that end with SSBM.

    Hex RegEx is done front to back, so both are used.


## Quantifiers

    Code Snipet: [a-f0-9]{6} Code Snipet: [a-f0-9]{3}


    Quantifiers define how many times a pattern of characters match. Quantifiers want to match as many occurrances of a pattern as they can, but if you set parameters using ?, it searches for as few as it can. Hex code is the former though.

    4{3} would equate to 444 (four repeated three times).

With Hex code, as the name suggests, 6 instances exist within the array values. It splits these up as 6 total characters in two groups of three.


## Grouping Constructs
    Grouping and Capturing: ()

    Code Snipet: ([a-f0-9]{6}|[a-f0-9]{3})

    The parenthesis group the REGEX between the opening and closing brackets. This treats many different characters as single objects. The function of grouping with parentheses is to dictate where to start and end parsing the Hex values.

    (test){5} would equate to testtesttesttesttesttest.

    Inside of the parenthesis though, is an array. The parenthesis group both arrays within. 

## Bracket Expressions
    Bracket Expression: []
    
    *Example: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

    Within the parenthesis, square brackets with characters inside come up next. These are to get all possible characters that you'd want to match to the desired result.


    *Code Snipet: [a-f0-9]

    In our reg ex, the bracket [] expression indicates matching a string that has any lower case character between a-f or any integer between 0-9

    Brackets signify regEx's that match patterns of characters with specificity. Hyphens are used to set specific ranges of characters. You can also use a ^ to negate values between your setpoints. 

## Character Classes
    Code Snipet: a-f0-9 Description: Character classes only matches one out of several characters defined in the character set. A hyphen can be used inside a character class to define a range of characters More than one range can be used -- as is the case in our code snipet.

    Example: [0-9] This character class matches a single digit between 0 and 9

    In our case, the character class consists of lower case a-f and/or integer 0-9


## The OR Operator
    OR Operator: |

    *Code Snipet: [a-f0-9]{6}|[a-f0-9]{3}

    The | symbol is a boolean value that searches for the expression both before and after it.

    5|2, for example, matches 222, 555, 525, and 252.

    In our case, that implies match with 3 character string containing lower case a-f and/or integer 0-9 OR a string with 6 characters containing lowercase a-f and/or integer between 0-9. A matching string has to have 3 or 6 character with the specified pattern. Anything other than 3 or 6 characters will not match.

## Flags

    Flags in RegEx's occur after the second / of the RegEx. Their function is to add more functionality or add limitations to the string. There aren't any for Hex though. Some examples of flags for other RegEx functions are the G flag, which globally searches and tests for matches, and the I flag, which functions as an ignore parameter.

    Flags occur after the second closing parentheses of the expression. They add more limits or functionality to the string of characters


## Character Escapes
    
    Character escapes are marked by a backslash, which basically makes any specific character into not what it actually is. If you had an expression that read \g\g\g, the letter of g will not be interpreted as a g.

### Author

Thank you for reading! You can add me on github and view my portfolio below:

GitHub: https://github.com/carsondipan

Portfolio: (link goes here)
