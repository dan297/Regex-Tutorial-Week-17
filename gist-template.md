# Regex Tutorial Week 17

## Introductory paragraph

This homework demonstrates Regex and provides a tutorial for use.
I had the option to choose from one of the following expressions

Matching a hex value
Matching an email
Matching a URL
Matching an HTML tag

I have chosen "Matching an email" and will give tutorials on how to match an Email address using Regular expression.

## Summary

According to Wikipedia, a regular expression is a sequence of characters that specifies a search pattern. Usually such patterns are used by string-searching algorithms for "find" or "find and replace" operations on strings, or for input validation. It is a technique developed in theoretical computer science and formal language theory.

Email matching regex.

Matching an Email: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Regex Tutorial Week 17](#regex-tutorial-week-17)
  - [Introductory paragraph](#introductory-paragraph)
  - [Summary](#summary)
  - [Table of Contents](#table-of-contents)
  - [Regex Components](#regex-components)
    - [Anchors](#anchors)
    - [Quantifiers](#quantifiers)
    - [Grouping Constructs](#grouping-constructs)
    - [Bracket Expressions](#bracket-expressions)
    - [Character Classes](#character-classes)
    - [The OR Operator](#the-or-operator)
    - [Flags](#flags)
    - [Character Escapes](#character-escapes)
  - [Author](#author)
  - [Questions](#questions)

## Regex Components

This section demonstrates the following Regex Components

### Anchors

Anchors have special meaning in regular expressions. 
The main job of an Anchor is to assert something about that string or the  matching process. Anchors assert that the engine's current position in the string matches a well-determined location: for instance, the beginning of the string, or the end of a line

To summarise, the '^' anchor is placed at the start of the text.
The '$' anchor is placed at the end of the text.
The rest of the code responsible for matching the email address is inside  these opening and closing anchors.

### Quantifiers

Quantifiers are used to match a number of instances of a character, group, or character class in a string.

Quantifiers match a number of instances of a character, group, or character class in a string.

The + operator will connect useers email name + email domain/address + .com.

Matching an Email: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Grouping Constructs

As mentioned  before, this particular Regex is constructed together using the '+' operator. 

In the email regex , you can divide the sequence into 3 groups.

Group #1: [a-z0-9_\.-]+) || This first group will match the user's email name before @ domain address.
Group #2: [\da-z\.-] || This second group will match the user's email domain or service they are using; such as @google or @yahoo
Group #3: [a-z\.]{2,6}. || This third will cover the ending of an email address; such as ".com or .net, etc..."


### Bracket Expressions

A braket expression represents a character set via a list of characters enclosed by the square brackets.
It normally matches the target string with any single character from the list.

In our email matching regex expression, Bracket expression includes the following character set `[a-z0-9_.-]. This is matching any letter a-z (case sensitive) and numbers 0-9 and matches the characters "_", ".", "."

### Character Classes

Character classes sets up a character and converts it into a number.
For this example the bracket expression : ([\da-z\.-]+) contains '\d' which represents the  number '4'.
It will only match a single digit such as "4", but not "44".

### The OR Operator

The 'OR' operator can be identified  with the '|' symbol. This however is not used in our email  exmaple. 

### Flags

Flags, in a regular expression, are tokens that modify its behavior of searching.
There are a total of 6 flags available in Javascript.

Flag i, which stands for ignore casing, does the job of carrying out a case-insensitive search.

Flag G, which stands for Global, makes the expression search for all occurences.

Flag S, which stands for Dot All, makes the wild character '.' match newlines as well.

Flag M, Which stands for Multiline,	makes the boundary characters ^ and $ match the beginning and ending of every single line instead of the beginning and ending of the whole string.

Flag Y, which stands for Sticky	, makes the expression start its searching from the index indicated in its lastIndex property.

Flag U, which stands for Unicode, Makes the expression assume individual characters as code points, not code units, and thus match 32-bit characters as well.

However in our code, no flags were used in email matching regex example.


### Character Escapes

Character escape was not used in email regex example however it is used when a backslash in a regular expression precedes a literal character.


## Author

Name: Daniel White

Aspirations: Looking  to grow my knowledge and become a full stack developer.

 ## Questions
  For any questions use the following contact information:
  - [Dan297](https://github.com/Dan297)
  - danielwhite98@icloud.com