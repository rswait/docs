# SQRT

**Created At:** 9/28/2017 10:50:33 AM  
**Updated At:** 1/5/2018 6:21:46 PM  


# Description

The **SQRT** function returns the mathematical square root of a value. It takes the form:

```
SQRT(expression)
```

Where:

expression should evaluate to a positive numeric value as the authors do not want to introduce a complex number type within the language. Negative values will cause a math error.

The function calculates the result at the highest precision available and then truncates the answer to the required [PRECISION](277629-precision).  An example of use would be:

```
PRECISION 2
CRT SQRT (44)
```

to display 6.63, which is the square root of 44 to 2 decimal places.

Go back to [jBASE BASIC](263498-jbase-basic).