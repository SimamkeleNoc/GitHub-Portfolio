# Agile Logbook — GuardPulse

## 1. Purpose

This logbook records development activities, observations, challenges, and lessons learned while building GuardPulse. It reflects my experience working independently on the project and identifies practices I would introduce to improve future development.

**Record note:** I worked on GuardPulse independently from start to finish. I did not maintain formal records of daily stand-ups or sprint meetings. The entries below are retrospective milestone reflections based on the project work and available evidence, not fabricated daily meeting records.

## 2. Development Milestones

### Milestone 1: Building the customer-facing storefront

**Activity:** Developed the storefront layout, navigation, and product catalogue for a South African online home-security store.

**Evidence:** [Homepage screenshot](evidence/01-guardpulse-homepage.png)

**Observation:** The homepage communicates the store's purpose and gives customers access to the main product categories.

**Reflection:** I learned that the user interface should make the purpose of the application clear and help customers navigate without unnecessary complexity. In future iterations, I would collect feedback from users to evaluate how easily they can find products.

### Milestone 2: Presenting the product catalogue

**Activity:** Worked on displaying products with images, names, descriptions, and prices.

**Evidence:** [Product catalogue screenshot](evidence/02-guardpulse-product-catalogue.png)

**Observation:** Product cards help customers compare available security products and bundles.

**Reflection:** Product presentation is an important part of an e-commerce application. Consistent product information and readable layouts help customers make informed decisions. I would continue checking product data and the layout across different screen sizes.

### Milestone 3: Implementing the shopping cart experience

**Activity:** Worked on the cart interface, including selected items, quantity controls, and the subtotal.

**Evidence:** [Shopping cart screenshot](evidence/03-guardpulse-cart.png)

**Observation:** The cart provides a summary of the selected product and its quantity before checkout.

**Reflection:** This stage highlighted the importance of keeping quantities and totals consistent as customers change their selections. I would continue using automated tests to check calculations and edge cases.

### Milestone 4: Integrating the checkout journey

**Activity:** Worked on the checkout experience, including customer details, the order summary, and an estimated delivery cost.

**Evidence:** [Checkout screenshot](evidence/04-guardpulse-checkout-redacted.png)

**Observation:** The checkout brings together order information and delivery estimates. The displayed shipping amount is an estimate, not a guarantee of the final charge.

**Reflection:** Checkout depends on several connected parts of the application. Validation, delivery-rate responses, and payment outcomes need to be handled carefully. PayFast remains in sandbox mode while account verification is pending, so the website is not yet accepting real payments.

### Milestone 5: Backend evolution and testing

**Activity:** Reworked the backend from Java and Spring Boot to TypeScript using Hono, with PostgreSQL hosted on Neon. The current backend has 25 automated tests, according to the project information recorded for this portfolio.

**Evidence:** The project repository, relevant GitHub commits, and test results can provide supporting technical evidence. The storefront screenshots alone do not prove backend test results.

**Reflection:** Changing the backend technology required attention to compatibility, configuration, and regression risks. This reinforced the value of testing existing functionality after significant architectural changes. In future work, I would record test results alongside each relevant change.

## 3. How I Organised My Work

I developed GuardPulse independently, completing features and fixing issues as I progressed. Git and GitHub commits provided a way to track changes and review the development history.

My approach was practical and iterative: work on a feature, examine the result, address issues, and continue with the next area of the application. However, I did not maintain a formal historical sprint log or daily stand-up record.

For this portfolio, I created a Product Backlog and a proposed Sprint Backlog to demonstrate how I would structure and prioritise future work. These documents represent retrospective planning and proposed practices, not proof that formal sprints were conducted.

## 4. Challenges and Risks

- **Backend migration:** Moving from Java and Spring Boot to TypeScript and Hono increased the importance of regression testing and configuration checks.
- **External integrations:** Shipping rates and payment processing depend partly on external services and account configuration.
- **Payment readiness:** PayFast is still in sandbox mode, so production payment readiness remains a limitation.
- **Independent workload:** Working alone meant I was responsible for implementation, testing, prioritisation, and resolving issues without a separate team member assigned to each responsibility.

## 5. Proposed Future Agile Practices

The following are practices I would introduce in future development. They are recommendations, not historical activities.

1. Maintain a prioritised backlog and update it as requirements change.
2. Define a clear goal and acceptance criteria for each sprint.
3. Track tasks as To do, In progress, Blocked, or Done.
4. Record development milestones and decisions as they happen.
5. Run automated tests before considering relevant tasks complete.
6. Conduct a short retrospective at the end of each iteration to identify improvements.
7. Attach screenshots, test output, and commit references to relevant tasks.

## 6. Overall Reflection

Building GuardPulse independently gave me experience across the customer-facing storefront, product catalogue, cart, checkout, backend development, and external integrations. It also demonstrated that completing a visible feature is only one part of delivering a reliable application. Testing, security, configuration, and external dependencies must also be considered.

The screenshots provide evidence of selected customer-facing features, while the code repository and test results can support claims about implementation and backend quality. A key improvement for future projects is to document decisions, task status, and test outcomes throughout development rather than reconstructing them later. This would make progress easier to evaluate and provide stronger evidence of how the work was completed.

## 7. Evidence Index

- [Homepage](evidence/01-guardpulse-homepage.png)
- [Product catalogue](evidence/02-guardpulse-product-catalogue.png)
- [Shopping cart](evidence/03-guardpulse-cart.png)
- [Checkout](evidence/04-guardpulse-checkout-redacted.png)
- [Agile Team Charter](Agile-Team-Charter.md)
- [Product Backlog](Product-Backlog.md)
- [Sprint Backlog](Sprint-Backlog.md)
- [User Stories and Tasks](User-Stories-and-Tasks.md)
