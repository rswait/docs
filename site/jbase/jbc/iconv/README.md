# ICONV

<PageHeader />

**Tags:**
<badge text='conversions' vertical='middle' />

## Description

The **ICONV()** function converts data in external form such as dates to their internal form. The function takes the general form:

```
ICONV(expression1, expression2)
```

Where:

- **expression1** evaluates to the data upon which the conversion is to be performed.
- **expression2** should evaluate to the conversion code that is to be performed against the data.

If the conversion code used assumes a numeric value and a non-numeric value is passed then the original value in **expression1** is returned unless the emulation option iconv\_nonnumeric\_return\_null is set.

An example of use is as:

```
InternalDate = ICONV("27 MAY 1997", "D")
CRT InternalDate
```

The above should display the date in internal format.

See also: [OCONV](./../oconv/README.md)

See also: [Conversion Processing](./../../conversion-processing/README.md)

Go back to [jBASE BASIC](./../README.md)

Go back to [Programmers' Reference Guide](./../../reference-guides/jbc/README.md)

<PageFooter />
