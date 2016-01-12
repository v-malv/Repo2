# codesnippet
Testing codesnippet page.

## Example 1

> [!div class="tabbedCodeSnippets" data-resources="OutlookServices.Calendar"]
> ```cs-i
var outlookClient = await CreateOutlookClientAsync("Calendar");
var events = await outlookClient.Me.Events
  .Take(10)
  .ExecuteAsync();
foreach(var calendarEvent in events.CurrentPage)
{
  System.Diagnostics.Debug.WriteLine("Event '{0}'.", calendarEvent.Subject);
}
 ```
>```javascript-i
outlookClient.me.events.getEvents().fetch().then(function (result) {
    result.currentPage.forEach(function (event) {
console.log('Event "' + event.subject + '"')
    });
}, function(error) {
    console.log(error);
});
```

## Example 2

> [!div class="tabbedCodeSnippets" data-resources="OutlookServices.Calendar"]
```cs-i
string string1 = "This is a string created by assignment.";
Console.WriteLine(string1);
string string2a = "The path is C:\\PublicDocuments\\Report1.doc";
Console.WriteLine(string2a);
string string2b = @"The path is C:\PublicDocuments\Report1.doc";
Console.WriteLine(string2b);
// The example displays the following output:
//       This is a string created by assignment.
//       The path is C:\PublicDocuments\Report1.doc
//       The path is C:\PublicDocuments\Report1.doc      
 ```

## Example 3

> [!div class="tabbedCodeSnippets" data-resources="OutlookServices.Calendar"]
> ```javascript-i
function inchestometers(inches)
   {
   if (inches < 0)
      return -1;
   else
      {
      var meters = inches / 39.37;
      return meters;
      }
   }
var inches = 12;
var meters = inchestometers(inches);
document.write("the value in meters is " + meters);
/*
> This is a multiline comment that explains the preceding code statement.
>
> The statement assigns a value to the aGoodIdea variable. The value, 
which is contained between the quote marks, is called a literal. A 
literal explicitly and directly contains information; it does not 
refer to the information indirectly. The quote marks are not part 
of the literal.
*/
```
