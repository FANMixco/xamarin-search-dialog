# xamarin-search-dialog
Android Search Dialog Library

![](https://i.stack.imgur.com/Z3GEx.png)

Example:

```csharp
var searchListItems = new List<SearchListItem>();
searchListItems.Add(new SearchListItem(1, "Tomatoes"));
searchListItems.Add(new SearchListItem(2, "Potatoes"));
searchListItems.Add(new SearchListItem(3, "Chili"));

//Context, List to display and Title
var searchableDialog = new SearchableDialog(this, SearchableDishes, "Search");
searchableDialog.OnSearchItemSelected = new SearchItemSelected();
searchableDialog.Show();

public class SearchItemSelected : Java.Lang.Object, IOnSearchItemSelected
{
	public void OnClick(int p0, SearchListItem p1)
	{
		Toast.MakeText(this, p1.Title, ToastLength.Long).Show();
	}
}
```

## Download

|  Package  |Latest Release|
|:----------|:------------:|
|**Xamarin.Search.Dialog**|[![NuGet Badge Xamarin.Search.Dialog](https://buildstats.info/nuget/Xamarin.Search.Dialog)](https://www.nuget.org/packages/Xamarin.Search.Dialog/)|
