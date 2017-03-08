```coldfusion
includedInObject(objectName, association, keys)
```
```coldfusion
// Check to see if the customer is subscribed to the Swimsuit Edition. Note that the order of the `keys` argument should match the order of the `customerid` and `publicationid` columns in the `subscriptions` join table
<cfif not includedInObject(objectName="customer", association="subscriptions", keys="#customer.key()#,#swimsuitEdition.id#")>
    assignSalesman(customer)>
</cfif>
```