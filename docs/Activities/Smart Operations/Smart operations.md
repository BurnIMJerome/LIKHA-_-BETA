# Smart Operations

![Likha Process Designer](../../images/process-designer.png)

These are rule-based smart operations powered by algorithms, regex, and fuzzy matching. They do not require AI integration.

## Activities

- [Similarity Score](Similarity%20Score.md)
- [Smart Equals](Smart%20Equals.md)
- [Normalize Text](Normalize%20Text.md)
- [Parse Human Number](Parse%20Human%20Number.md)
- [Compare Currency](Compare%20Currency.md)
- [Detect Number Format](Detect%20Number%20Format.md)
- [Fuzzy Company Match](Fuzzy%20Company%20Match.md)
- [Extract Invoice Number](Extract%20Invoice%20Number.md)

## Summary

### Similarity Score

Compares two text values and returns a Number score from 0 to 100.

### Smart Equals

Normalizes two text values and returns true when their fuzzy score is greater than or equal to the threshold.

### Normalize Text

Applies lowercase, punctuation cleanup, and whitespace cleanup.

### Parse Human Number

Parses compact number text such as `15k`, `2.5M`, or `1 billion`.

### Compare Currency

Strips currency symbols and compares two decimal amounts using a tolerance.

### Detect Number Format

Detects common rule-based formats such as integer, decimal dot, decimal comma, thousands comma, thousands dot, human abbreviated, or currency.

### Fuzzy Company Match

Normalizes company names, removes common legal suffixes, and fuzzy-matches the remaining names.

### Extract Invoice Number

Uses regex patterns to extract invoice numbers from text.

