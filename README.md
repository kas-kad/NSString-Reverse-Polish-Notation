NSString-Reverse-Polish-Notation
================================

This category allows you to evaluate the infix/postfix-notation expressions, convert infix-notation expression to postfix one.

###Examples:
- To evaluate infix-notation expresson "(2.4+7.1)*3.1/3^2-(1.2^4.3+6^3)":

```
NSString * infixExp = @"(2.4+7.1)*3.1/3^2-(1.2^4.3+6^3)";
double result = [infixExp evaluateInfixNotationString];
```

- To evaluate postfix-notation expresion "2.4 7.1 + 3.1 * 3 2 ^ / 1.2 4.3 ^ 6 3 ^ + -":

```
NSString * postfixExp = @"2.4 7.1 + 3.1 * 3 2 ^ / 1.2 4.3 ^ 6 3 ^ + -";
double result = [postfixExp evaluatePostfixNotationString];
```

- To convert expression from infix- to postfix-notation:

```
NSString * infixExp = @"(2.4+7.1)*3.1/3^2-(1.2^4.3+6^3)";
NSString * postfixExp = [infixExp infixToPostfixWithOutputDecimalSeparator: nil];
```
