# Regex tutorial for hex code matcher
in this readMe we will discuss the following regex code:
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
its the code to check that a hex code matches.
the componets of the code will be broken down to explain it in this read me.

## Summary
the regex code i chose for this is the following:

> /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ 

its the code used to check that two hex codes are matching below we will break apart each component to explain what each part does and how it all works together to achive its goal.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)

## Regex Components

### Anchors
the following is the anchor portion of the line of code
> /^#

the anchor exist to stat the start of the expression and checks that it mataches what is being compared against so in the snippit above it checks to make sure that it starts with the ***#*** matches againt what it is being compared to in this insatance its used as that is what is used to start a hex code also at the end of the snippit the $ sign also acts as an anchor however this one exist to single the end of the code so its encased within the ^ and the $ it also work similar to the opening anchor to ensure the item before it is included  and matches

### Quantifiers
the following is the quantifier section of the code
> /^#?

more specificly its the question mark part at the end of the snippit it is here to say that the character before it is optional so the hashtag here may not be neccesiary as part of the comparison so when being compared agasint another hex code that doesnt start with # it can still work but also accounts for if the # is being used

### Grouping Constructs
the following is the grouping constructs of the snippit 
> ([a-f0-9]{6}|[a-f0-9]{3})

more speciffcily its the parenthsis () this is necessary to have because it groups parts together to be referanced later as a single entity 


### Bracket Expressions
the following is the bracket expressions of the snippit
> [a-f0-9]

its the square bracket on either end of the snippit [] it exist to check if something is there that fits within the range for example [3-6] check that the item in this section falls between the numbers 3 and 6 including the 3 and 6 in its check this is useful to see that the data fits within the peramiters in this example of using a hex code hex goes from a-f and 0-9 to help denote the color in the hex code

### Character Classes
the following is the character classes of the snippit
> a-f0-9

in this instance here it is very similar to the bracket expression its allowing a range of chaarcters to be chosen or allowed to be used to check agaisnt another set so in this insatnce it can be a letter between a and f or a number between 0 and 9


### The OR Operator
the following is the OR operator of the snippit
> [a-f0-9]{6}|[a-f0-9]{3}

in this instance here it the | after the 6 in curly brackets what this does is it acts as comparison operator it checks that the thing to the left of the line can match up with the stuff on the right of the line its what does our comparing to make sure it matches up 

### Flags
This code does not contain flags however as a brief overview to keep an eye out in the future Flags exist to change the default search behavior of the expression they are denoted with a lowercase letter such as i, g, m to list a few depedning on what letter is used it modifies the search behavior in different ways

## Author
My name is Alex Ryder this is my github page https://github.com/Zorzorac05
I made this document to clear up confusion others may have with regular expressions so that people can better understand and read them going forward
