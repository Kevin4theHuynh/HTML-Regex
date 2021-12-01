# Regux Tutorial

Hello I am Khoa Huynh and I will be explaining Regux (regular expressions) matching an HTML

## Summary
Regux (regular expressions) is a special text string for for describing a search pattern. By using special characters such as 
`^.*.txt$` allows you to find all text files in file manager. This is similar to `.txt` 

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
With Anchors in HTML tags they match position by string not by chracter

`^` : Matches the beginning of the string 
`\w`: Matches the word character
### Quantifiers

### Grouping Constructs
Matching a pair of opening and closing HTML tags, and the text between has become easier by using parentheses and some text inside. The first backslash matches the first captured group and the second backslash will match the exact text that was referenced by the first backslash.
Ex. `([j-l]x1x/1)`
This will match `jxjxj`, `kxkxk`, `lxlxl`
The number behind the foward slash is not limited to 1 this could go up to as high as 99 

### Bracket Expressions

### Character Classes
Negated set: Will select any letter character that is not in the set string 
Ex: [^eo]
Ex: Hello world! I enjoy eating food
This will include H,L,W,R,D,J,N,O,F,I,F

### The OR Operator

### Flags
The multiline anchor matches the beginning and the end of a line. With the pattern `[/^\d/gm]`

Ex: Const str = `Sally ate food`
`Billy Sleeping`
`Kevin is coding`
`console.log( str.match(/^\d/gm)` // S, B, K

This also works with the $
Ex:`[/\d$gm]`

Without the m and $ the whole text will be matched.

### Character Escapes
Octal matches a character in the sequence with the same value that is passed in. This includes numbers that are single digit, double digit, or triple digit. However this will not work if the number is 000 also the value must be less than /251. This is passed with the special character ©
Ex: `[/252]` this number and anything higher will not work
Ex: `Currently I am ©21 years old`
This will pass

Ex2: `Currently I am ©252 years old` 
This will not pass

## Author
 My name is Khoa Huynh but I go by Kevin with friends and co-workers. I was originally an English major in college but found a higher interest in coding. 
 [Link]: https://github.com/Kevin4theHuynh
