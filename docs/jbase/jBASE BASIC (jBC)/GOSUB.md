# GOSUB

**Created At:** 9/6/2017 2:20:18 PM  
**Updated At:** 6/10/2019 9:34:03 AM  

**Tags:**
<badge text='gosubstackdepth' vertical='middle' />

# Description

The **GOSUB** statement causes execution of a local subroutine, after which execution will continue with the next line of code.

```
GOSUB label
```

Where **label** refer to an existing label within the current source code.



## Notes: 


> The compiler does not check for the existence of a [RETURN](278787-return) statement and if no [RETURN](278787-return) statement is encountered the program will continue until the final statement and not return to the original **GOSUB**.




An example of use is as:

```
GOSUB Initialize ;* open files etc..
GOSUB Main ;* perform main program
GOSUB Finish ;* close files etc..
STOP
...
Initialize: * open files
OPEN......
.
RETURN
....
Main: * main execution loop
......
RETURN
Finish: * clean up after execution
......
RETURN
```



Go back to [jBASE BASIC](263498-jbase-basic).