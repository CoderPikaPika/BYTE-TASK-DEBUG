the staff & student window is same allows a studnt to change the menu items

### CC-01 : "The search suggestions are behind everything"

**Reproduced:** used inspect and tried searching for uttapam, the suggestion box was behind the cat-tab.
**Cause:** the z-index of parent level cat-tab was overshadowing the suggestion box .

**Fix:** removed the z-index on cat-tab after proper check so that it does not effect rest of the ui.

**Checked:** used inspect to check the css for filter filter-inner cat-tab and rest inside the "filter" div in section.

**Time:** about 35 minutes, around 15 minutes to understand the issue and finding it in the ui and 10-15 minutes to solve the problem after analysing the consequences of the change i was doing.

### CC-02: "Can't read anything in dark mode"

**Reproduced:** used inspect and tried to check the source of error
**Cause:** the color :var(--ink) was not assigned in dark mode to dish-name zand dish price

**Fix:** assigned both values in thier respective classes

**Checked:** used inspect and tried to check the all relavant classes like dish-name dish-price

**Time:** about 15 minutes

### CC-06: "I ordered more than they had"

**Reproduced:** tried ordering many times
**Cause:** no stock check

**Fix:** added stock check and limited state of cart so that frontend can only set atmost maxstock and a backend check in validation

**Checked:** cart.js dish.js menu.js state.js validate.js and related backend functions

**Time:** about 1:30 hours on frontend and 20-25 minutes on backend

### CC-07: "Cancelling makes it worse"

**Reproduced:** tried cancelling to understand issues
**Cause:** arithmetic issue in validationjs backend relsaestock function

**Fix:** changed - to +

**Checked:** order related files

**Time:** about 10 minutes

## Example — delete this

### CC-99 — "The cart total is wrong"

**Reproduced:** Added 2 dosas at Rs. 60 each. The cart showed
Rs. 119.99999 instead of Rs. 130. Happened every time, on any dish with
a price ending in .50.

**Cause:** The total was being added up with plain floating point and
never rounded, so 0.1 + 0.2 style errors showed up on screen. The
rounding helper existed but this one place was not using it.

**Fix:** Ran the total through the existing rounding helper instead of
adding a new one, so every price on screen goes through the same path.

**Checked:** Cart, checkout and the order screen all show Rs. 130 now.
Prices without decimals still show without a trailing .00.

**Time:** about 40 minutes, most of it working out that the cart and the
order screen round in different places.

## CC-0X — "<the complaint, in short>"

**Reproduced:**

**Cause:**

**Fix:**

**Checked:**

**Time:**

## Could not fix

For anything you investigated but did not solve. Say what you tried and
where you got to. This is worth marks — leaving it blank when you got
stuck is not.

### CC-0X — "<the complaint>"

**What I tried:**

**Where I got to:**

**What I would try next:**

## Extra credit

Anything not on the bug log: a problem you found yourself, a test you
wrote, or a fix you are unsure about. Same format, plus one line on how
you noticed it.
