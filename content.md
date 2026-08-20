The assignment operator (typically `=`) is one of the most fundamental operations in programming. While it looks similar to the equals sign in mathematics, it works very differently and is worth understanding in depth.

# Evaluation Order: Right Before Left

Assignment always follows the same pattern: the expression on the right-hand side is evaluated first, and then the result is assigned to the variable on the left.

```
x = 5
y = x + 3       // Step 1: Evaluate x + 3 (which is 8)
                // Step 2: Store 8 in y

x = x * 2       // Step 1: Evaluate x * 2 (which is 10)
                // Step 2: Store 10 back in x
```

# Assignable Locations

The left-hand side of an assignment must be an <strong>assignable location</strong>—often a variable. You cannot assign to literal values or arbitrary expressions:

```
x = 5               // ✓ Valid: x is a variable
10 = x              // ✗ Invalid: 10 is a literal
x + 3 = y           // ✗ Invalid: x + 3 is an expression
```
