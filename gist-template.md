# Matching a URL Regex tutorial jth

Searching for a matching URL in a string

## Summary


Client side validation

The below set of code is used to verify that the user is submitting the correct URL format in the text box to validate that this is a true statement

Matching a URL: 
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
/^ determines the start of the search for the correct string, whereas $/ is used to denote the end of the search for the corresponding string. You can see these used at the beginning, and end of the code.
### Quantifiers
*,?,+,{} - These symbols define how many matches can be made

{2,6} in the string is used to determine that between 2, and 6 matches must be made
* is used to define that the match occurs 0 or more times, and is short for {0,}
? is used to determine that 1 or less matches are made, and is short for {0,1}
+ is used to determine that 1 or more matches are made, and is short for {1,0}
### Grouping Constructs
() - The parentheses are used to group the corresponding matches in the string, these can be seen in:

-(https?:\/\/)
-([\da-z\.-]+)
-([a-z\.]{2,6})
-([\/\w \.-]*)
### Bracket Expressions
[] - Matches any string that has any character defined within the brackets.

-[a-z\.] matches a single character in the range between a & z with a character.
-[\da-z\.-] matches a single character in the range between a & z, before one digit equivalent to [0-9] & the characters 
-[\/\w \.-] - this bracket expression indicates that any slash, any alphanumeric character, a dot, or a hyphen will produce a match
### Character Classes
-. - Matches any character except for /n (new line)

-/d - Matches any numerical digit

-/w - Matches any alphanumeric character from the latin 
alphabet, including an underscore (_)

-/s - Matches a single whitespace character, including tabs and line breaks

-[\da-z\.-] - /d is being used to indicate any number will product a match within this bracket expression(character class).
-[\/\w \.-] - /w is being used to indicate any letter will produce a match in this bracket expression
### Character Escapes
-\. - Used to indicate that we're looking for the character, and not the character class

Created by Jordan Heidlage

Github: https://github.com/jordanheidlage
