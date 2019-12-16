# REWIND

**Created At:** 9/28/2017 7:46:37 AM  
**Updated At:** 1/5/2018 6:11:35 PM  


# Description

The **REWIND** statement will issue a rewind command to the device attached to the specified channel. It takes the general form:

```
REWIND{ON expression} THEN|ELSE statements
```

Where:

expression, if specified, should evaluate to an integer in the range 0 to 9. Default is 0.

## Note:


> If the statement fails to issue the rewind then any statements associated with the ELSE clause are executed. If the statement successfully issues the rewind command then the statements associated with any THEN clause are executed. Either or both of the THEN and ELSE clauses must be specified with the statement.
> 
> If the statement fails then the reason for failure can be determined via the value of [SYSTEM(0)](282982-system-functions) as follows:
> 
> 
> | Value<br> | Meaning<br> |
> | --- | --- |
> | 1<br> | there is no media attached to the channel<br> |
> | 2<br> | an end of file mark was found<br> |


Go back  to [jBASE BASIC](263498-jbase-basic).