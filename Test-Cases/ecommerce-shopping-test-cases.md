# E-commerce Shopping Test Cases

## Test Case 1: Add Product to Cart
**Test Case ID:** TC_SHOP_001  
**Priority:** High  
**Test Type:** Functional

### Pre-conditions:
- User must be logged in
- Product must be in stock

### Test Steps:
1. Login to website
2. Browse to a product category
3. Select a product
4. Click "Add to Cart" button
5. View shopping cart

### Expected Result:
- Product added to cart successfully
- Cart icon shows updated count
- Price displayed correctly in cart
- Success notification: "Product added to cart"

### Actual Result:
Pass ✅

---

## Test Case 2: Remove Product from Cart
**Test Case ID:** TC_SHOP_002  
**Priority:** High  
**Test Type:** Functional

### Test Steps:
1. Add a product to cart
2. Go to cart page
3. Click "Remove" or trash icon for the product
4. Confirm removal if prompted

### Expected Result:
- Product removed from cart
- Cart total updated correctly
- Cart count decreased by 1
- Confirmation message shown

### Actual Result:
Pass ✅

---

## Test Case 3: Update Product Quantity in Cart
**Test Case ID:** TC_SHOP_003  
**Priority:** High  
**Test Type:** Functional

### Test Steps:
1. Add a product to cart (quantity: 1)
2. Go to cart page
3. Change quantity to 3
4. Click "Update" button

### Expected Result:
- Quantity updated to 3
- Price multiplied by 3 correctly
- Cart total recalculated
- Stock availability verified
- Message: "Cart updated successfully"

### Actual Result:
Pass ✅

---

## Test Case 4: Proceed to Checkout
**Test Case ID:** TC_SHOP_004  
**Priority:** High  
**Test Type:** Functional

### Test Steps:
1. Add products to cart (total: $100)
2. Click "Proceed to Checkout" button
3. Verify redirect to checkout page

### Expected Result:
- User redirected to checkout page
- Order summary displayed
- Shipping address form shown
- Cart items and total visible

### Actual Result:
Pass ✅

---

## Test Case 5: Complete Order with Valid Payment
**Test Case ID:** TC_SHOP_005  
**Priority:** Critical  
**Test Type:** End-to-End

### Test Steps:
1. Add products to cart
2. Proceed to checkout
3. Enter valid shipping address
4. Select shipping method
5. Select payment method: Credit Card
6. Enter valid card details
7. Click "Place Order"

### Expected Result:
- Order placed successfully
- Order confirmation page displayed
- Order number generated
- Confirmation email sent
- Payment processed
- Inventory updated

### Actual Result:
Pass ✅

---

## Test Case 6: Apply Valid Coupon Code
**Test Case ID:** TC_SHOP_006  
**Priority:** Medium  
**Test Type:** Functional

### Test Steps:
1. Add products worth $100 to cart
2. Go to cart page
3. Enter coupon code: SAVE10 (10% off)
4. Click "Apply Coupon"

### Expected Result:
- Coupon applied successfully
- Discount: $10 (10% of $100)
- New total: $90
- Success message: "Coupon applied successfully"
- Coupon code displayed in order summary

### Actual Result:
Pass ✅

---

## Test Case 7: Invalid Coupon Code
**Test Case ID:** TC_SHOP_007  
**Priority:** Medium  
**Test Type:** Negative

### Test Steps:
1. Add products to cart
2. Enter invalid coupon code: INVALID999
3. Click "Apply Coupon"

### Expected Result:
- Error message: "Invalid coupon code"
- No discount applied
- Original price remains
- Coupon field highlighted in red

### Actual Result:
Pass ✅

---

## Test Case 8: Empty Shopping Cart
**Test Case ID:** TC_SHOP_008  
**Priority:** Low  
**Test Type:** Functional

### Test Steps:
1. Go to shopping cart page when cart is empty
2. Observe the page

### Expected Result:
- Message: "Your cart is empty"
- "Continue Shopping" button displayed
- No checkout option available

### Actual Result:
Pass ✅

---

## Test Case 9: Product Out of Stock
**Test Case ID:** TC_SHOP_009  
**Priority:** High  
**Test Type:** Negative

### Test Steps:
1. Navigate to a product that is out of stock
2. Try to add to cart

### Expected Result:
- "Out of Stock" badge displayed
- "Add to Cart" button disabled or hidden
- "Notify Me" option available
- Cannot add product to cart

### Actual Result:
Pass ✅

---

## Test Case 10: Save Items for Later
**Test Case ID:** TC_SHOP_010  
**Priority:** Low  
**Test Type:** Functional

### Test Steps:
1. Add products to cart
2. Click "Save for Later" on one product
3. Check saved items section

### Expected Result:
- Product moved to "Saved for Later"
- Product removed from cart
- Cart total updated
- Can move item back to cart

### Actual Result:
Pass ✅

---

## Summary
- Total Test Cases: 10
- Passed: 10
- Failed: 0
- Success Rate: 100%

## Test Coverage
- Add to Cart: ✅
- Remove from Cart: ✅
- Update Quantity: ✅
- Checkout Process: ✅
- Payment: ✅
- Coupon Codes: ✅
- Stock Management: ✅
