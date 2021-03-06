# jCL F-DELETE

<PageHeader />

**Tags:**
<badge text='file' vertical='middle' />
<badge text='record' vertical='middle' />
<badge text='delete' vertical='middle' />
<badge text='jcl' vertical='middle' />

## Description

The command deletes a record from a file. It takes the general form:

```
F-DELETE file-buffer
```

or

```
F-D file-buffer
```

where **file-buffer** is the number (1 to 9) of the file buffer, which is associated with the file containing the record to be deleted.

## Note

> The record specified in field zero (&f.0) of the file buffer will be deleted. If the record does not exist, the command will have no effect. The content of the file buffer is not altered and any outstanding record lock will be released. The file must have been opened with an F-OPEN  command.

### Example

```
PQN
10 T "File name :",+
IBP %1
F-O 1 %1
T "File ", %1, " does not exist!"\ GO  10
MV &1.0 "Key"
F-D 1
```

If the file cannot be opened by the F-O command, the line immediately following the command will be executed (see the F-O command). If the file is opened, "Key" is moved into field 0 of file buffer 1. F-D 1 then attempts to delete record "Key" from the file.

Back to [jCL.](./../README.md)
  
<PageFooter />