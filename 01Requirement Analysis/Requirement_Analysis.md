
1. Introduction
This document captures the understanding of functional requirements of the OpenCart demo e-commerce application. The goal is to analyze system features before test design begins.

// The application allows users to register, log in, browse products, add items to the cart, and complete purchases.

2. Application Overview

OpenCart is an online shopping platform where users can:
Create an account
Log in to their account
Search and view products
Add products to shopping cart
Complete checkout process

3. Modules Identified
Module	Description
Registration -->New user account creation.
Login -->	Existing user authentication.
Product Search -->	Searching products using keywords.
Product Details -->	Viewing product info and adding to cart.
Cart -->Managing selected products.
Checkout -->Completing order process.
4. Functional Requirement Understanding

----------//------
4.1 Registration Module

User should be able to create a new account.

*Fields observed:

        First Name
        Last Name
        Email Address
        Telephone
        Password
        Confirm Password
        Privacy Policy checkbox (mandatory)
        System Behavior:
        All mandatory fields must be filled
        Email should be unique
        Password and Confirm Password must match
        On successful registration → account creation confirmation

4.2 Login Module

Existing users should be able to log in.
Inputs:

Email and Password
Features:
        Login button
        Forgotten Password link
        System Behavior:
        Valid credentials --> user dashboard
        Invalid credentials --> error message

4.3 Product Search Module

Users should be able to search products.
Functionality: 
        Search bar available
        Keyword-based search
        Expected Behavior:

Matching products displayed
No match → appropriate message

4.4 Product Details Page

Users can view product information.
Details Available:
Product image
Product name
Price
Description
Quantity selection
Add to Cart button

4.5 Cart Module

Users manage added products.
Features:
View products in cart
Update quantity
Remove product
View total price

4.6 Checkout Module

Users complete purchase.
Steps Observed:
Login or Guest checkout option
Billing details entry
Delivery method selection
Payment method selection
Order confirmation

5. User Flow Identified

User registers
User logs in
User searches for product
User views product details
User adds product to cart
User proceeds to checkout
User places order

6. Assumptions

Application is web-based
Functional testing focus only
Payment gateway behavior may be simulated

7. Areas to Clarify (if real project)

Password complexity rules
Email format validation rules
Max cart quantity allowed
Guest checkout restrictions

8. Conclusion

The application supports a complete online shopping workflow. These identified modules and flows will be used for test scenario and test case design in the next phase.