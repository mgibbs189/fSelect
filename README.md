# fSelect
A jQuery select box replacement library ([live demo](https://jsfiddle.net/r0pw7g11/3/))

<img src="http://i.imgur.com/yXOv8DG.png" width="208" height="223" />

### Usage

```javascript
$('.your-select-box').fSelect();
```

### Available options

```javascript
$('.your-select-box').fSelect({
    placeholder: 'Select some options',
    numDisplayed: 3,
    overflowText: '{n} selected',
    noResultsText: 'No results found',
    searchText: 'Search',
    showSearch: true
});
```

* **placeholder** (str) - the default placeholder text
* **numDisplayed** (int) - the number of values to show before switching to the `overflowText`
* **overflowText** (str) - the text to show after exceeding the `numDisplayed` limit
* **noResultsText** (str) - the text to show if no choices exist (or an empty string)
* **searchText** (str) - the search box placeholder text
* **showSearch** (bool) - show the search box?

### Single vs. multi-select

Add the `multiple` attribute to your `<select>` to enable multi-select:

```html
<select class="your-select-box" multiple="multiple">
```
