# Conditionals in Python
## *1. What values in Python are considered false?*
- None (basic data type)
- False (basic data type)
- Any empty sequence: '', [], ()
- Any zero value: 0, 0.0
- Anything whose len() returns 0
- Empty objects
- Everything else is True

## *2. What is a chain comparison? Give an example with and without using chaining.*
Chain comparison is using multiple comparators on the same line
```python
# Using chaining
x = 3
1 < x < 5
# No chaining
x = 10
x > 5
x < 15
```

## *3. What is the meaning of short-circuit evaluation?*
Short-circuit evaluation occurs becuase python evaultes expressions from left to right. As soon as it knows enough to stop evaluating, it stops, even if some operands have not been looked at yet.

## *4. Why is the expression 'A' < 'a' true?*
Because the ACSII value for "a" is greater than the ASCII value for "A"