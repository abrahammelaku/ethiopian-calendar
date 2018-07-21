# Ethiopian Calendar
Example code to convert Gregorian to Ethiopian
```csharp
var grDate = new DateTime(2018, 09, 10);
var etCal = new EthiopianCalendar();
var etDateString = string.Format("{0}-{1}-{2}", 
  etCal.GetYear(grDate).ToString("D4"),
  etCal.GetMonth(grDate).ToString("D2"),
  etCal.GetDayOfMonth(grDate).ToString("D2"));
Console.WriteLine(etDateString); //prints 2010-13-05
```
Example code to convert Ethiopian to Gregorian
```csharp
var grDate = new DateTime(2011, 1, 1, new EthiopianCalendar());
Console.WriteLine(grDate.ToString("yyyy-MM-dd")); //prints 2018-09-11
```
