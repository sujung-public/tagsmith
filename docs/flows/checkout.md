# Checkout funnel requirements

Part of the [Northwind Outfitters analytics requirements](../requirements.md).

The checkout has four steps on a single-page app (URL does not change between steps):

| Step | Name | Notes |
|---|---|---|
| 1 | Shipping | address entry; guests may choose "Create an account" |
| 2 | Delivery | standard / express / store pickup |
| 3 | Payment | card, PayPal, Apple Pay, gift card |
| 4 | Review | final review before "Place order" |

## Requirements

- Track checkout start when the visitor lands on step 1, and each step view with the step name.
- Track the selected delivery method and payment method.
- Track checkout errors (payment declined, invalid address) with the error message, without any personal data.
- On the order confirmation page track the order: order ID, revenue, tax, shipping cost, units, and each product (SKU, quantity, price).
- Track coupon code usage (code + discount amount) and gift card usage.
- Track whether the order was placed as a guest or a logged-in member, and first vs. repeat purchase.
- Track checkout abandonment: last checkout step reached when the visitor leaves without ordering.
