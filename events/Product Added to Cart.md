# Product Added to Cart

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Product Added to Cart",
    "cart": {
        "cartModifications": "<cartModifications>"
    },
    "eventDetails": {
        "multiAdditionDetail": "<multiAdditionDetail>",
        "multiAdditions": "<multiAdditions>"
    },
    "product": [
        {
            "fulfillment": {
                "isBopusOnly": "<isBopusOnly>"
            },
            "price": {
                "sellingPrice": "<sellingPrice>"
            },
            "productInfo": {
                "isOffer": "<isOffer>",
                "isOutOfStock": "<isOutOfStock>",
                "productID": "<productID>",
                "thirdyPartyVendorID": "<thirdyPartyVendorID>"
            },
            "quantity": "<quantity>"
        }
    ]
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|cartModifications|integer|Count of times the change in product quantity was the result of a cart modification.||||||||
|isBopusOnly|integer|Count of times the user engaged with a product whose only available shipping method was Buy Online Pick Up In Store \(i.e., BOPUS\).||||||||
|isOffer|integer|Count of times an offered product \(e.g., Gift with Purchase, Purchase with Purchase\) is added to the cart.||||||||
|isOutOfStock|boolean|Boolean flag indicating that an inventoried product is out of stock. |TRUE, FALSE|||||||
|multiAdditionDetail|string|Provides details of multiple product additions to carts, wishlists, registries, etc.|all items, 3 of 5, 2 of 4|||||||
|multiAdditions|boolean|Flag indicating whether multilple products where added to carts, wishlists, registries, etc.|true, false|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|quantity|integer|Integer number of products being acted upon \(added to a cart, removed from wishlist, purchased, reserved\)|1, 2, 3, 4, 5||||1|||
|sellingPrice|string|String representation of the price paid after coupons or discounts. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|thirdyPartyVendorID|string|Captures the vendor id of the third party vendor associated with product conversion.||||||||
