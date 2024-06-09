# xamarin-search-dialog
Android Search Dialog Library

![](https://i.sstatic.net/Z3GEx.png)

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

### Follow me at:

|  LinkedIn  |YouTube|Amazon|Goodreads|Instagram|Cyber Prophets|Sharing Your Stories|
|:----------|:------------:|:------------:|:------------:|:------------:|:------------:|:------------:|
|[![LinkedIn](https://i.sstatic.net/idQWu.png)](https://bit.ly/lfanmixco)|[![YouTube](https://i.sstatic.net/CFPMR.png)](https://youtube.com/c/FedericoNavarrete)|[![Amazon](https://i.sstatic.net/NFOeE.png)](https://www.amazon.com/Federico-Navarrete/e/B08NJTXQRV)|[![Goodreads](https://i.sstatic.net/oBk0g.jpg)](https://www.goodreads.com/author/show/21125413.Federico_Navarrete)|[![Instagram](https://i.sstatic.net/PIfqY.png)](https://www.instagram.com/federico_the_consultant)|[![RedCircle Podcast](https://i.sstatic.net/4XICF.png)](https://redcircle.com/shows/cyber-prophets)|[![RedCircle Podcast](https://i.sstatic.net/4XICF.png)](https://redcircle.com/shows/sharing-your-stories)|
