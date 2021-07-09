# Checkout Interaction Occurred

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Checkout Interaction Occurred",
    "checkoutInteraction": {
        "interactionType": "<interactionType>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|interactionType|string|Type of click event engaged with by the user on the checkout page.||||||||
