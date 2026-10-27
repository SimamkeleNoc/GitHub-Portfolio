# Product Backlog — GuardPulse

## 1. Purpose

The product backlog is a prioritised list of features, improvements, and technical work relevant to GuardPulse. It helps identify what should be developed, verified, or improved to provide value to customers and support store operations.

**Documentation note:** This backlog is being documented for the PRP370S portfolio. Its priorities represent a proposed planning order, not a historical backlog or proof that formal sprint planning occurred.

## 2. Product Vision

GuardPulse aims to provide South African customers with a convenient online store for security cameras and related home-security products. Customers should be able to explore products, manage a cart, understand delivery costs, and complete the supported order process. The store owner should be able to manage products, stock, orders, and customers.

The store currently has 59 products across 11 categories. The frontend uses React, TypeScript, and Vite; the backend has been rewritten from Java and Spring Boot to TypeScript using Hono. PostgreSQL is hosted on Neon. The frontend is hosted on Netlify and the backend on Vercel.

## 3. Prioritised Backlog

| ID | Backlog item | Priority | Value or reason |
|---|---|---|---|
| PB01 | Verify product catalogue and category browsing | High | Helps customers find suitable products |
| PB02 | Verify cart calculations and checkout validation | High | Supports a reliable shopping journey |
| PB03 | Verify The Courier Guy delivery-rate integration | High | Helps customers understand delivery costs |
| PB04 | Complete PayFast production readiness | High | Needed before accepting real payments |
| PB05 | Verify registration, sign-in, and password reset | High | Supports customer account access |
| PB06 | Verify order creation and stock handling | High | Supports reliable order processing |
| PB07 | Verify administrative product, order, stock, and customer management | High | Supports store operations |
| PB08 | Verify order emails and notification handling | Medium | Keeps customers informed |
| PB09 | Verify customer order history and status display | Medium | Helps customers follow their purchases |
| PB10 | Verify product review functionality | Medium | Supports customer feedback |
| PB11 | Maintain and expand automated backend tests | High | Helps detect regressions and improve reliability |
| PB12 | Review backend rewrite and deployment configuration | Medium | Helps maintain the TypeScript backend |
| PB13 | Improve error handling and user-facing messages | Medium | Helps customers understand unsuccessful operations |
| PB14 | Review security, privacy, and access controls | High | Protects accounts, orders, and administrative operations |

## 4. Current Constraints and Known Status

- GuardPulse is live at [guardpulse.co.za](https://guardpulse.co.za).
- The frontend is hosted on Netlify.
- The TypeScript/Hono backend is deployed on Vercel.
- PostgreSQL is hosted on Neon.
- The current backend has 25 automated tests, according to the project information recorded for this portfolio.
- PayFast remains in sandbox mode while account verification is pending. Real payments are not yet enabled.

These details describe the reported project state. The backlog items above still need to be checked against the current implementation before being labelled complete or incomplete.

## 5. Proposed Definition of Done

A backlog item may be considered complete when:

1. The required functionality has been implemented.
2. Relevant input validation and error handling are in place.
3. Appropriate automated or manual tests have been completed.
4. The change does not introduce known regressions in related functionality.
5. Supporting evidence, such as test results or screenshots, is available.
6. Any limitations or dependencies are documented.

For payment-related work, production readiness must also account for PayFast account verification, production configuration, and appropriate end-to-end checks before real payments are enabled.

## 6. Reflection

Creating this backlog helps me organise GuardPulse work according to customer value, operational needs, and technical risk. It also makes the distinction between implementing a feature and verifying its reliability clearer.

The payment integration illustrates why prioritisation must account for external dependencies. Although the payment flow has been integrated, the application cannot yet accept real payments because PayFast remains in sandbox mode. This means that production readiness requires more than code changes alone.

In future development, I would review the backlog regularly, assign clear acceptance criteria, record implementation status, and reprioritise items when technical risks or external dependencies change. This would make progress easier to measure and help ensure that important work is not overlooked.

## 7. Supporting Evidence

Possible evidence includes:

- Storefront screenshots showing products and categories.
- Relevant cart, checkout, and delivery-rate functionality.
- PayFast sandbox configuration or test evidence, with secrets removed.
- GitHub commits documenting implementation changes.
- Automated test results.
- Administrative functionality and order-management screenshots.

Only label an item as implemented, tested, or complete when current project evidence supports that status.
