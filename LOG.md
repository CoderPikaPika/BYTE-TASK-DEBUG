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

### CC-03: "The menu is wider than my phone"

**Reproduced:** used inspect and resposive designs found the issue at 550px
**Cause:** the media for ,menu-grid was improper

**Fix:** used min-max to improve the ui

**Checked:** different devices a few custom and responsiveness on inspect

**Time:** about 20 minutes

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

### CC-08: "An old coupon still works"

**Reproduced:** tried out all the coupons from coupon.json

**Cause:** logical error in backend and frontend not checking expired coupons after use

**Fix:** fixed frontend and added backend logic in pricing.js

**Checked:** frontend backend files related to coupons

**Time:** about 40 minutes

### CC-10: "Sorting by price is backwards"

**Reproduced:** tried sorting in phone tablet and laptop mode

**Cause:** logical error in backend sorters was assigned incorrectly

**Fix:** swapped sorters for price-asc and price-desc

**Checked:** menu.routes menu.js search.js
**Time:** about 30 minutes

### CC-11: "Coupon after use did not update its count on use cancelling was fine "

**Reproduced:** tried out all the coupons from coupon.json

**Cause:** logical error in backend and frontend not updating coupon usesleft properly

**Fix:** fixed frontend and updated backend logic in orders.routes

**Checked:** Cart, checkout and the order screen all show Rs. 130 now.
Prices without decimals still show without a trailing .00.

**Time:** about 40 minutes, most of it working out that the cart and the

### CC-12 — "the staff & student window is same allows a student to change the menu items & stock"

**What I tried:** Authentication system can be built so that discounts coupons and admin systems can be persnalised.

**Where I got to:** I did not solve this problem due to lack of time

**What I would try next:**

### CC-13 — "order tokens are saved but orders not shown on my orders"

**What I tried:** Authentication system can be built so that discounts coupons and admin systems can be persnalised.

**Where I got to:** I did not solve this problem due to lack of time

**What I would try next:**

### CC-12 — ""

**What I tried:** Authentication system can be built so that discounts coupons and admin systems can be persnalised.

**Where I got to:** I did not solve this problem due to lack of time

**What I would try next:**
