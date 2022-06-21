# The Expression of Matching a Hex Value

The purpose of this challenge was to find a regular expression used in coding (Regex) and break down it's components.

## Summary

The Regex being explained in this GIST is the expression used for matching a hex value: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

## Table of Contents

- [Forward Slash](#forward-slash)
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Range](#range)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)

## Regex Components

### Forward Slash
The purpose of forward slashes in the expression are to state the beginning and the end of the expression.

### Anchors
The ^ symbol is an anchor used to indicate the start of a string.

### Quantifiers
'#' matches the character with an index. The ? will by default match a value between 0 an 1 as many times as it possibly can. 

### OR Operator
This regex does not have an or operator. 

### Character Classes
The '[]' identify a character within a group. In this case [a-f0-9]

### Flags
Flags are optional parameters that can be added to a regex that will modify it's behavior. 

### Range
The ranges being compare in this expression are a-f, 'a' having an index of 97 and 'f' having an idex of 102, as well as 0-9, '0' having an index of 48 and '9' having an idex of 57.

### Grouping and Capturing
Grouping is used to unify a pattern so that multiple tokens will be processed together as a single unit. 

### Bracket Expressions
The brackets '()' are used to match everything enclosed inside of them into a group. 

### Greedy and Lazy Match
This match will be identified by the '?'. A greedy match will match the previous token as many times as needed.

### Boundaries
Boundaries are the spaces between the characters but are not actual characters. , = a boundary: /,^,#,?,(,[,a,-,f,0,-,9,],{,6,},|,[,a,-,f,0,-,9,],{,3,},),$,/

### Back-references
Back-references means to reference something that has already been captured. In this regex, the characters on the left side of the {6} are being back referenced when being compared to the characters on the right side. 


## Author

This GIST was written by Cory Sillaots, a current student in the University of Toronto SCS Coding Boot Camp.
You can visit Cory's github profile at [Github](https://github.com/CorySillaots?tab=repositories)