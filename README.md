# Caem Configurator

## Shelfing Types
Pick between the following
- TN9
- S50
- M25
- Ardente
- Uni Zinc
- BTC

Each of them have their own set of products for each category outlined below.

## Uprights
Presents a list of items for each Upright Height size

- 148
- 156
- 180
- 200
- 224
- 236
- 288

1 per unit quantity. These don't care about Unit Type.

## Bases

Again we have preset sizes for base depth.

Here though if the Unit type is Gondola (or Gondola Endset) we need to add 2 of this product per unit quanity.

## Gondola Top Covers

These are only relevant to Gondola Unit Types, not Gondola Endset.

Question Pitch is aligned with the Size of this top cover.

This only applies if the upright height is less than 180.

> Why is this linked to 180? This doesn't seem relevant to the Upright that has been chosen.

> is 180 an arbitary number?

If it meets the above condiutions its 1 product quantity per Unit Quantity

## Plain Back Panels

> How does this calculate the quantity? I have put in a height of 224 pitch of 65 and the panels are 4 * 44, 1 * 24 and 1 * 8 which leaves me with 204 if you add the heights, but if I had 4 * 44 and 2 * 24 it would leave me exactly 224. For this to be viable I need to be able to mathematically calculate how many panels the base requires. If this can't work like this I will have to come up with a system for Caem to add "rules" to each product they add for back panels, which can get messy. 

Generate an algorithm to calculate what panels are required. 

Pitch = Size column 2

## Perforated Back Panels

Matches with Pitch, multiples the quantity with the amount the customer wants. No other calculation here.

## Shelf Planks

Matches with Pitch. 

> How is this calcualted? I can't break down the Excel If Function easily

## Brackets

Matches it's size with the Shelf Depth question and mutliples its by 2 for Wall or 4 for Gondola.

> There are 2 Shelf Depth/Qty questions on the sheet, is this correct? 

> Will there ever be more than 2, or less than 2?

## Kickers

Matches with Pitch and mutliplies by Unit Quantity. Double for Gondola

## Drop Plates

Same Calc as Kickers, can just use that value.

## Epos

Matches with Pitch, 1 per shelf quantity and 1 per unit, so 4 shelves and 1 unit is a total of 5. Gondolas are doubled.

## Fixings

> Some of these are blank, are we making them all blank? Or only if it can't calculate a fixing. We need some way of knowing what or how to calc.

## Base Covers and Upright Side Covers

These are blank.

## Programming Questions
> Can we get the price out of the Caem product DB?

> How are we linking each of the products to a Type/Category (TN9/Uprights)?

> How are they configured to know if a product has a multipler (i.e. this product requires 2 per base)?

> Gondolas are just walls * 2??
