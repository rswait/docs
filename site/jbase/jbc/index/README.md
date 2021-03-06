# INDEX

<PageHeader />

## Description

The **INDEX** function will return the position of a character or characters within another string. It takes the general form:

```
INDEX(expression1, expression2, expression3)
```

Where:

- **expression1** evaluates to the string to be searched.
- **expression2** evaluates to the string or character that will be searched for within **expression1**.
- **expression3** should evaluate to an integer value and specify which occurrence of **expression2** should be searched for within **expression1**.

## Note

> If the specified occurrence of **expression2** is not found in **expression1** then it returns Zero (0).

An example of use is as:

```
alphbt = "abcdefghijklmnopqrstuvwxyzabc"
CRT INDEX(alphbt , "a", 1)
CRT INDEX(alphbt , "a", 2)
CRT INDEX(alphbt, "jkl", 1)
```

to display:

```
1
27
10
```

Go back to [jBASE BASIC](./../README.md)

Go back to [Programmers' Reference Guide](./../../reference-guides/jbc/README.md)

<PageFooter />
