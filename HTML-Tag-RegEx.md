# Regular Expression for Matching HTML Tags

This regular expression can be used to match HTML tags in a string. It matches opening and closing tags, as well as self-closing tags.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

`const regex = /<([a-z][a-z0-9]*)\b[^>]*>(.*?)<\/\1>|<([a-z][a-z0-9]*)\b[^\/]*\/?>/gi;`

# Explanation
The regular expression consists of two parts separated by the | operator:

* `<([a-z][a-z0-9]*)\b[^>]*>(.*?)<\/\1>` matches opening and closing tags.
* `<([a-z][a-z0-9]*)` matches the opening tag and captures the tag name in a capturing group.
* `\b[^>]*` matches any attributes of the tag.
* `>(.*?)<\/\1>` matches the contents of the tag and the closing tag, using a non-greedy match for the contents and a backreference to the captured tag name.
* `<([a-z][a-z0-9]*)\b[^\/]*\/?>` matches self-closing tags.
* `<([a-z][a-z0-9]*)` matches the tag and captures the tag name in a capturing group.
* `\b[^\/]*` matches any attributes of the tag, but not the closing / character.
* `\/?>` matches the closing / character for self-closing tags, or the > character for non-self-closing tags.
* The regular expression is case-insensitive (i flag) and global (g flag) to match all occurrences in a string.








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

### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
