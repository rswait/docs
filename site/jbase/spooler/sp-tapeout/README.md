# SP-TAPEOUT

<PageHeader />

**Tags:**
<badge text='spooler tape ' vertical='middle' />

## Description

Reads spooled print jobs from a tape device and requeues them to the current formqueue assignment. The command takes the general form:

```
SP-TAPEOUT (n
```

where **n** is the number of print jobs to read and requeue.

## Example

Attach the tape device using the [T-ATT](./../../tape/t-att/README.md) command and use [T-FWD](./../../tape/t-fwd), if required, to position the tape media to the required print job record.

Assign the required formqueue by using the SP-ASSIGN command.

Execute the SP-TAPEOUT command.

```
SP-TAPEOUT (4
```

This command will read the next four print job files and spool them to the currently assigned formqueue.

Back to [Spooler](./../jbase-spooler).

<PageFooter />
