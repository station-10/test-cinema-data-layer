# Onsite Search Performed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.eventDataLayer = window.eventDataLayer || [];
eventDataLayer.push({
  "event": "Onsite Search Performed",
    "onsiteSearch": {
        "keyword": {
            "searchTerm": "<searchTerm>"
        }
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|searchTerm|string|Describes the search keyword used after auto-correct, auto-complete, or keyword suggestion. |bluth, blue, red lobster|||||||



