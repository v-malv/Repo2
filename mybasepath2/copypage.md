---
Title: Outlook Calendar REST API reference
---

# copypage


## <a id="Swagger"> </a> Swagger


[!code-REST-i[trydata](try/trydata.json)]


## <a id="Code_table"> </a>Code table


<!-- BEGINSECTION class="tabbedCodeSnippets" data-resources="OutlookServices.Calendar" -->
```cs-i
var outlookClient = await CreateOutlookClientAsync("Calendar");
var events = await outlookClient.Me.Events
  .Take(10)
  .ExecuteAsync();
 
foreach(var calendarEvent in events.CurrentPage)
{
  System.Diagnostics.Debug.WriteLine("Event '{0}'.", calendarEvent.Subject);
}
 
```
```javascript-i
outlookClient.me.events.getEvents().fetch().then(function (result) {
    result.currentPage.forEach(function (event) {
console.log('Event "' + event.subject + '"')
    });
}, function(error) {
    console.log(error);
});
```
```fs-i
using namespace System;
void main()
{
   String^ string1 = "This is a string created by assignment.";
   Console::WriteLine(string1);
   String^ string2a = "The path is C:\\PublicDocuments\\Report1.doc";
   Console::WriteLine(string2a);
}
```
<!-- ENDSECTION -->


##NOTE
> [!NOTE]
> This is NOTE

The above is NOTE text

> [!WARNING]
> This is WARNING

The above is WARNING text

> [!TIP]
> This is TIP

The above is TIP text

> [!IMPORTANT]
> This is IMPORTANT

The above is IMPORTANT text

> [!CAUTION]
> This is CAUTION

The above is CAUTION text

If any question, please contact me~

## <a> </a>Responsive Table
Scenario  |Permission
------------- | ------------- |
Password Sync| <li>Replicate Directory Changes.</li>  <li>Replicate Directory Changes All.</li>
Exchange Hybrid Deployment|See [Office 365 Exchange Hybrid AAD Sync write-back attributes and permissions](https://msdn.microsoft.com/library/azure/dn757602.aspx#exchange).
Password Write-back | <li>Change Password</li><li>Reset password</li>
User, Group, and Device Write-back|Write permissions to the directory objects and attributes that you wish to 'write-back'
Single Sign-On and AD FS| Domain admin permissions in the domain in which your federated servers are located. 
