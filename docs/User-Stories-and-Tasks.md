# User Stories and Tasks — GuardPulse

## 1. Purpose

This document describes key user stories for GuardPulse, a South African online store for security cameras and related home-security products. Each story describes a user need and provides tasks and acceptance criteria that can guide implementation and testing.

**Documentation note:** These stories and tasks are documented for this portfolio. They should not be interpreted as proof that formal user-story planning took place during the original development.

## 2. User Stories

### US01 — Browse Products

**As a** customer,  
**I want** to browse security products by category,  
**so that** I can find products that meet my home-security needs.

**Tasks**
- Display available products in the storefront.
- Organise products into categories.
- Present relevant product information.
- Verify that product listings and category navigation work.

**Acceptance criteria**
- Customers can view available products.
- Products can be explored through the available categories.
- Product information is displayed clearly.

### US02 — Manage a Shopping Cart

**As a** customer,  
**I want** to add products to my cart and review the selected items,  
**so that** I can prepare an order before checkout.

**Tasks**
- Implement adding products to the cart.
- Display selected items and quantities.
- Allow customers to review or update their selections.
- Check that cart totals reflect the selected items.

**Acceptance criteria**
- A customer can add an available product to the cart.
- The cart displays the selected products and quantities.
- The displayed total updates when the cart changes.

### US03 — View Delivery Prices

**As a** customer,  
**I want** to see delivery prices based on my address,  
**so that** I can understand the shipping cost before placing an order.

**Tasks**
- Collect the required delivery information.
- Request shipping rates through The Courier Guy integration.
- Display returned delivery options and prices.
- Handle unsuccessful rate requests appropriately.

**Acceptance criteria**
- The system can request delivery rates using the required address information.
- Returned rates are presented to the customer.
- If rates cannot be retrieved, the customer receives an appropriate indication.

### US04 — Place an Order

**As a** customer,  
**I want** to complete the checkout process,  
**so that** I can submit an order for the products I selected.

**Tasks**
- Validate the required checkout information.
- Check product availability and stock.
- Calculate the order total.
- Integrate the payment flow with PayFast.
- Verify order handling for successful and unsuccessful payment outcomes.

**Acceptance criteria**
- Required checkout information is validated.
- The order total reflects the selected products and applicable delivery cost.
- Payment outcomes are handled appropriately.
- The current PayFast sandbox limitation is clearly communicated; real payments are not yet enabled.

### US05 — Manage an Account

**As a** customer,  
**I want** to register, sign in, and reset my password,  
**so that** I can access account-related features securely.

**Tasks**
- Implement account registration and authentication.
- Validate user input.
- Provide a password-reset process.
- Test relevant account flows.

**Acceptance criteria**
- Users can complete the supported registration and sign-in flows.
- Invalid input is handled appropriately.
- Password-reset functionality provides a suitable recovery process.

### US06 — Track Orders

**As a** customer,  
**I want** to view my orders and their status,  
**so that** I can follow the progress of my purchases.

**Tasks**
- Associate orders with the appropriate customer account.
- Provide an order-history view.
- Display available order-status information.
- Check that customers cannot access another customer's order information.

**Acceptance criteria**
- An authenticated customer can view their own available order information.
- Order details are restricted to the appropriate customer.
- Status information reflects the data available in the application.

### US07 — Leave a Product Review

**As a** customer,  
**I want** to submit a product review,  
**so that** I can share feedback about a product.

**Tasks**
- Provide a product-review submission flow.
- Validate review information.
- Store and display reviews according to the application's rules.
- Test invalid submissions.

**Acceptance criteria**
- A valid review can be submitted through the supported functionality.
- Invalid review information is handled appropriately.
- Reviews are displayed according to the application's rules.

### US08 — Manage the Store

**As an** administrator,  
**I want** to manage products, orders, stock, and customers,  
**so that** I can maintain the online store.

**Tasks**
- Provide the relevant administrative views and operations.
- Support product and stock management.
- Support order management.
- Apply appropriate access controls.
- Test important administrative operations.

**Acceptance criteria**
- An authorised administrator can access the supported management functions.
- Product, stock, and order changes are handled correctly.
- Administrative functions are protected from unauthorised access.

## 3. Prioritisation

The following is a proposed priority order for future planning, not a historical sprint plan:

| Priority | User stories | Reason |
|---|---|---|
| High | US01, US02, US04 | Core shopping and checkout journey |
| High | US03 | Delivery pricing supports checkout decisions |
| High | US05, US08 | Account access and store administration |
| Medium | US06, US07 | Order visibility and customer feedback |

Actual implementation status should be checked against the current application before any story is marked complete.

## 4. Reflection

Writing these user stories helps me view GuardPulse from the perspectives of customers and administrators instead of focusing only on code. It makes the expected behaviour of each feature clearer and provides acceptance criteria that can guide testing.

A lesson I take from this exercise is that implementing a feature is only one part of development. The expected user outcome, error handling, access control, and testing also need attention. In future iterations, I would connect each story to smaller tasks, measurable acceptance criteria, test evidence, and a recorded status so that progress is easier to evaluate.

## 5. Supporting Evidence

Relevant evidence may include storefront screenshots, checkout and delivery-rate tests, account-related functionality, administrative screens, GitHub commits, and automated test results. Only mark a story as implemented or tested when the current code or other evidence supports that claim.
