# Title (Matching a Phone Number with Regex)

Regular expressions are a powerful tool for finding patterns in text data, 
and one common use case is matching phone numbers in various formats. 
In this tutorial, we will focus on matching phone numbers in the format of (123) 456-7890 using a regex pattern. 
We will break down the different components of this pattern, including anchors, quantifiers, and character classes, 
and explain how they work together to match the phone number.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Summary](#Summary)

## Regex Components

### Anchors
Anchors are special characters that match the position of a string rather than specific characters within it. 
In our phone number regex pattern, we use the caret (^) and dollar sign ($) as anchors. 
The caret matches the start of the string, and the dollar sign matches the end of the string. 
Using these anchors ensures that the phone number is matched in its entirety and not just a portion of it.

### Quantifiers
Quantifiers are used to specify how many times a character or group of characters should be matched. 
In our phone number regex pattern, we use the \d (digit) character class with the {3} and {4} quantifiers to match the area code 
and last four digits of the phone number, respectively. 
We also use the space and hyphen characters to match the specific formatting of the phone number.

### Character Classes
Character classes are used to match specific types of characters within a string. 
In our phone number regex pattern, we use the \d (digit) character class to match any digit from 0 to 9. 
e also use the space and hyphen characters to match the specific formatting of the phone number.

### Grouping and Capturing
Grouping and capturing are used to capture specific portions of a string that match a pattern. 
In our phone number regex pattern, we use parentheses to group the area code and the last four digits of the phone number, 
allowing us to capture these portions of the phone number as separate groups. 
We also use back-references to ensure that the opening and closing parentheses of the area code match each other.

### Summary

In summary, the regex pattern we use to match phone numbers in the format of (123) 456-7890 is: ^\d3\d3 \d{3}-\d{4}$


The various components of this pattern work together to match the specific pattern of the phone number. 
Anchors ensure that the entire string is matched, quantifiers and character classes specify the specific formatting of the phone number,
and grouping and back-references ensure that the opening and closing parentheses of the area code match each other.

## Author

Written by Mason Aviano github:https://github.com/Wodaloo