# MerchantPOS

An independent restaurant POS prototype built to demonstrate merchant workflow understanding for a sales interview.

## Try the demo

Open `index.html` in a browser. Keep `app.js` beside it. No installation is required.

For GitHub Pages, deploy from the `main` branch and the `/ (root)` folder in repository Settings → Pages.

## Demo walkthrough

1. Add a burger and a drink to an order.
2. Capture a guest request and split the check evenly.
3. Simulate a declined card: the order remains intact, and no sale is recorded.
4. Complete a simulated sale and view Merchant insights.
5. Open Demo guide for discovery questions and technical talking points.

## Technical choices

- Buildless HTML, CSS, and JavaScript.
- Monetary calculations use whole cents; split checks allocate remaining cents, so shares total correctly.
- A successful simulated sale adds a transaction to reporting.
- Browser local storage retains completed transactions on that browser and origin.
- No card data is collected, and no payment processor is connected.

## Scope and limitations

This is a portfolio prototype, not production POS software or an official product. The 7% tax rate is illustrative. Guest requests are captured in the order but are not routed to a kitchen. Check splitting calculates shares; it does not process individual guest payments. Browser storage can be cleared and is not a shared database.

A production system would need server-side payment verification, duplicate-charge prevention, authentication and staff permissions, a shared database, supported terminal integration, and operational monitoring. Payment authorization and settlement are separate stages that this prototype does not implement.

## Validation

JavaScript syntax checked. Full browser interaction testing is pending.
