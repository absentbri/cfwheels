```coldfusion
setPrimaryKey(property)
```
```coldfusion
// In `models/User.cfc`, define the primary key as a column called `userID`
<cffunction name="init">
    setPrimaryKey("userID")>
</cffunction>
```