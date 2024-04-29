# Hex Value Matcher

I will be breaking down the Hex Value Matcher (`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`)

## Summary

The regex `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/` will find all hex values.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors

The `^` and `$` are the anchor tags in the regex. The `^` indicates the start and `$` indicates the ending.

### Quantifiers

The quantifiers are `?`, `{6}`, and `{3}`.

The `?` will match `#` zero or one time(s).  
The `{6}` will match `[a-f0-9]` exactly six times.  
The `{3}` will match `[a-f0-9]` three times. As far as hex color codes go, this syntax is only valid with repeating values, such as `#bbaadd` being shortened to `#bad` (🕺🏾shamone!)

### OR Operator

The `|` (OR Operator) allows either side of it to be true. In this case, it's `[a-f0-9]{6}` or `[a-f0-9]{3}`.

### Grouping and Capturing

The `()` (Grouping Construct) is `([a-f0-9]{6}|[a-f0-9]{3})`. In this specific regex, the grouping construct is practically the entire expression, since the beginning of it only says that the `#` may or may not be there.

### Bracket Expressions

The `[a-f0-9]` is the bracket expression and it evaluates whether a string contains only the letters `a` through `f` and/or numbers 0 to 9.

## Author

My name is Adam Huss and I'm a Full-Stack Web Development student. Here is my other work: [Github](https://github.com/AHuss13)
