# Event Booking Started

### 

## Javascript Code
```js
window.eventDataLayer = window.eventDataLayer || [];
eventDataLayer.push({
  "event": "Event Booking Started",
    "booking": {
        "ticketList": [
            {
                "event": {
                    "eventId": "<eventId>",
                    "eventName": "<eventName>",
                    "eventType": "<eventType>",
                    "fakeProductId": "<fakeProductId>",
                    "startDate": "<startDate>",
                    "startTime": "<startTime>",
                    "ticketType": "<ticketType>"
                },
                "price": {
                    "sellingPrice": "<sellingPrice>"
                },
                "quantity": "<quantity>"
            }
        ]
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|eventId|string|Unique Identifier of an event. |155, 65588, 987764448|||||||
|eventName|string|The friendly name of the event.|Max your 401K, Structured JavaScript, Mid Day Yoga, Frosty 5K Fun Run, Whiskey Wednesday|||||||
|eventType|string|The type of the event|Webinar, Class, Conference, Race, Meet Up|||||||
|fakeProductId|string|Helper node used by AA Product String Builder to set product to location. This field gets a static value of "event".  With updates to the AA PS extension, this will soon go away.|event|event||||||
|quantity|integer|Integer number of products being acted upon \(added to a cart, removed from wishlist, purchased, reserved\)|1, 2, 3, 4, 5||||1|||
|sellingPrice|string|String representation of the price paid after coupons or discounts. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|startDate|string|Start date. ISO 8601 form \(YYYY-MM-DD\). Jan 1, 2019 is 2019-01-01|2001-12-22, 2011-01-01|^([0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])$||||||
|startTime|string|Start Time. 24H format zero padded.|10:30, 14:45, 23:59, 07:00|^[0-2][0-9]:[0-5][0-9] ||||||
|ticketType|string|General type of ticket for an event. May be used as needed.|Adult, Family, Student, Senior, All Access, General Admission|||||||



