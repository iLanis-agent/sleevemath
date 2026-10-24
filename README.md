# Sleeve Math

Event workshop bagel sleeve, week, cost and time arithmetic. The 340 bagels at 8 bagels a sleeve take 43 sleeves, the last sleeve holding 4 bagels.

## Named constants

None. Every number is the owner's own entry.

## What it computes

- **The sleeves truth** - the bagels (1 to 1000000) divided by the bagels a sleeve (1 to 1000), rounded up, with what the last sleeve holds.
- **The weeks truth** - the bagels divided by the bagels used a week (1 to 100000), with the bagels left for the next week.
- **The cost truth** - the sleeves (1 to 100000) times the sleeve price ($0.01 to $999.99) to the cent, and spread over the bagels, half rounded up.
- **The time truth** - the bagels divided by the bagels packed a minute (1 to 100), rounded up, in minutes and in hours and minutes.

## Boundary

Arithmetic only. Counting applied as written. It has not seen any bagel, sleeve or venue and does not know whether bagels will really stay fresh, a supplier will run out or a price will hold, and it gives no verdict that a sleeve is worth its price or a bagel is right for an event. Every number is the owner's own entry.

## Files

- `index.html` - landing page with the boundary and starting examples.
- `app.html` - the calculator; every sleeve recomputes on each keystroke.
- `engine.js` - the four truths, shared by the page and the tests.
- `oracle.py` - an independent Python re-implementation; writes `expected.json`.
- `test.js` - runs the engine against `expected.json` (99 cases, 20 error cases).

## Tests

```
python3 oracle.py
node test.js
```
