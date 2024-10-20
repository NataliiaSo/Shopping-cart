# Shopping Cart Project

## Overview
This simple online shop project allows users to add items to a cart, increase or decrease quantities, remove items, and proceed with checkout. The application is built using JavaScript, with all functionality related to products, the cart, and checkout implemented in `script.js`. Optional functionality may be added by uncommenting sections in `front.js`.

## Features
- Add items to the cart: Clicking an item adds it to the cart and increases its quantity when clicked multiple times.
- Increase, decrease, or remove items from the cart.
- Checkout functionality: Calculates the total cost of items in the cart and processes payments.

## Folder Structure
The folder structure of the project remains unchanged. All JavaScript functionality is implemented in `script.js`, and if optional features are added, the bonus sections in `front.js` can be uncommented.

## Product Array
A minimum of three product objects are created in an array named `products` in `script.js`. Each product object contains the following properties:
- `name` (string): The name of the product.
- `price` (number): The price of the product.
- `quantity` (number): Initially set to zero.
- `productId` (number): A unique ID for the product.
- `image` (string): A URL string for the product image.

## Functionality

### Cart Functionality
The following functions are implemented to manage the cart:
- **`addProductToCart(productId)`**: Adds a product to the cart. If the product is already in the cart, its quantity is increased.
- **`increaseQuantity(productId)`**: Increases the quantity of a product in the cart.
- **`decreaseQuantity(productId)`**: Decreases the quantity of a product. If the quantity reaches 1, the product is removed from the cart.
- **`removeProductFromCart(productId)`**: Removes the product entirely from the cart.

### Checkout Functionality
Two main functions handle the checkout process:
- **`cartTotal()`**: Calculates and returns the total cost of all products in the cart.
- **`pay(amount)`**: Takes the amount paid by the user and returns the positive or negative balance depending on whether the amount covers the total cost.

### Global Variable
A global variable is used to hold the remaining balance after the `pay()` function is called.

## JavaScript Best Practices
- The code follows modern JavaScript practices, using `let` and `const` instead of `var`.
- Consistent indentation (2 spaces) is used throughout the code.
- Meaningful variable and function names are chosen to enhance readability.
- Console logs used for debugging have been removed.
- Helper functions are used to avoid code repetition.
- The code is documented with concise comments explaining key sections.

## Usage
1. Open the project in a browser to view the live shop page.
2. Add items to the cart by clicking on product images or names.
3. Adjust the quantity of items in the cart by using the increase or decrease buttons.
4. Remove items from the cart entirely by clicking the remove button.
5. Proceed to checkout by entering the payment amount and calculating the remaining balance.
