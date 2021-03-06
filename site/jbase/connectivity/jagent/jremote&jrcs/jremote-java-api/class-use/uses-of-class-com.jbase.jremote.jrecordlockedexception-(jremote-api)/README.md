# Uses of Class com.jbase.jremote.JRecordLockedException (jremote API)

<PageHeader />

## Uses of Class
com.jbase.jremote.JRecordLockedException

| Package<br> | Description<br> |
| --- | --- |
 Packages that use [JRecordLockedException](./../../jrecordlockedexception-(jremote-api) "class in com.jbase.jremote")  | com.jbase.jremote<br> |  <br> |
| com.jbase.jremote.io<br> |  <br> |





### Uses of [JRecordLockedException](./../../jrecordlockedexception-(jremote-api) "class in com.jbase.jremote") in [com.jbase.jremote](./../../../../jremote-api)


| Modifier and Type<br> | Method and Description<br> |
| --- | --- |
 Methods in [com.jbase.jremote](./../../../../jremote-api) that throw [JRecordLockedException](./../../jrecordlockedexception-(jremote-api) "class in com.jbase.jremote")  | `JDynArray`<br> | JFile.`readU(String recordKey, boolean blockedRead)`<br>Read a record where the supplied recordKey is the key to the record and locks it for update.<br> |
| `boolean`<br> | JFile.`writeU(String recordKey, JDynArray record, boolean blockedWrite)`<br>Write the supplied record to the jBASE file.<br> |






### Uses of [JRecordLockedException](./../../jrecordlockedexception-(jremote-api) "class in com.jbase.jremote") in [com.jbase.jremote.io](./../../io/com.jbase.jremote.io-(jremote---api))


| Modifier and Type<br> | Method and Description<br> |
| --- | --- |
 Methods in [com.jbase.jremote.io](./../../io/com.jbase.jremote.io-(jremote---api)) that throw [JRecordLockedException](./../../jrecordlockedexception-(jremote-api) "class in com.jbase.jremote")  | `JDynArray`<br> | JFileImpl.`readU(String recordKey, boolean blockedRead)` <br> |
| `boolean`<br> | JFileImpl.`writeU(String recordKey, JDynArray record, boolean blockedWrite)` <br> |

Back to [jRemote API](../../../../jremote-api/README.md)

  
<PageFooter />
