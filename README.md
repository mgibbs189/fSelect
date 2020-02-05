# fSelect
A jQuery select box replacement library ([live demo](https://facetwp.com/wp-content/plugins/facetwp/assets/vendor/fSelect/test.html))

<img src="http://i.imgur.com/yXOv8DG.png" width="208" height="223" />

### Usage

```javascript
$('.your-select').fSelect();
```

### Available options

```js
$('.your-select').fSelect({
    placeholder: 'Select some options',
    numDisplayed: 3,
    overflowText: '{n} selected',
    noResultsText: 'No results found',
    searchText: 'Search',
    showSearch: true,
    showSelectAll: true,
    multiSelect: false
});
```

* **placeholder** (str) - the default placeholder text
* **numDisplayed** (int) - the number of values to show before switching to the `overflowText`
* **overflowText** (str) - the text to show after exceeding the `numDisplayed` limit
* **noResultsText** (str) - the text to show if no choices exist (or an empty string)
* **searchText** (str) - the search box placeholder text
* **showSearch** (bool) - show the search box?
* **showSelectAll** (bool) - show select-all option? (only with multiSelect)
* **multiSelect** (bool) - initialize with multi-select enabled (works the same as select attribute)

### Methods

```js
$('.your-select').fSelect('reload');
$('.your-select').fSelect('destroy');
```

### Single vs. multi-select

Add the `multiple` attribute to your `<select>` to enable multi-select (optional; can set in fSelect options OR in select tag):

```html
<select class="your-select-box" multiple="multiple">
```
