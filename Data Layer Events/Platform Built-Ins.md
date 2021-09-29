# Platform Built-Ins

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.eventDataLayer = window.eventDataLayer || [];
eventDataLayer.push({
  "event": "Platform Built-Ins"
});
```







