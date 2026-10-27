# Agile Team Charter — GuardPulse

## 1. Project Overview

**Project:** GuardPulse  
**Developer:** Simamkele Talent Nocuze  
**Working arrangement:** Individual development

GuardPulse is a South African e-commerce store for security cameras and related home-security products. It serves customers who want to explore and purchase security products online, with delivery pricing based on their address.

## 2. Project Purpose

The purpose of GuardPulse is to provide an online platform where customers can browse security products, manage their shopping carts, place orders, and access account-related features. The system also supports administrative management of products, orders, stock, and customers.

The store currently lists 59 products across 11 categories. Its payment integration remains in PayFast sandbox mode while account verification is pending, so real payments are not yet enabled.

## 3. Roles and Responsibilities

I developed GuardPulse independently from start to finish and was responsible for planning and implementing its functionality, investigating technical issues, and improving the application.

My work included:

- Developing the frontend using React, TypeScript, and Vite.
- Developing the backend, initially using Java and Spring Boot and later rewriting it in TypeScript using Hono.
- Working with PostgreSQL through Neon.
- Implementing e-commerce functionality, including cart, checkout, and stock management.
- Integrating delivery-rate functionality with The Courier Guy.
- Working with PayFast payment integration and order-related emails.
- Implementing customer account functionality and product reviews.
- Developing and testing backend functionality, with 25 automated tests reported for the current backend.
- Tracking code changes using Git and GitHub.

The frontend is hosted on Netlify, and the TypeScript backend is deployed on Vercel.

## 4. Working Approach

I worked independently in stages, implementing features and resolving issues as development progressed. Rather than relying on a formal team-based Scrum process, I managed the development work myself and used Git and GitHub commits to track code changes.

The transition from Java and Spring Boot to TypeScript and Hono also reflects how the project evolved technically. This change required adapting the backend implementation while continuing to develop the overall application.

## 5. Working Principles

The principles that guide my work on GuardPulse are:

- **Incremental development:** Work on features in manageable stages.
- **Accountability:** Take responsibility for implementation, debugging, and testing.
- **Quality assurance:** Use automated tests and investigate problems found during development.
- **Version control:** Use Git and GitHub commits to track code changes.
- **Maintainability:** Keep the application organised as its technologies and functionality evolve.
- **Transparency:** Distinguish completed functionality from features that remain limited or incomplete.

## 6. Proposed Future Agile Practices

The following practices are proposed improvements for future development. They are not claims that formal Scrum ceremonies or records were maintained throughout the project:

- Maintain a prioritised product backlog.
- Define a clear goal for each development iteration.
- Break features into tasks with measurable acceptance criteria.
- Record progress, blockers, and test results.
- Review completed work against its acceptance criteria.
- Conduct retrospectives to identify lessons and improvements after each iteration.

## 7. Reflection

Developing GuardPulse independently gave me experience in managing different parts of a software application, including frontend development, backend architecture, database integration, checkout functionality, and testing. Working in stages helped me address technical issues as they arose, while Git and GitHub commits provided a record of code changes.

Rewriting the backend from Java and Spring Boot to TypeScript and Hono was an important example of adapting the technical direction of a project. It reinforced the importance of understanding the consequences of architectural changes and verifying functionality after implementation.

One area I can improve is the formal documentation of planning and progress. Although I tracked code changes, structured backlogs, iteration goals, and retrospectives would make the development process easier to evaluate. I intend to apply these practices in future work to improve planning, traceability, and continuous improvement.

## 8. Supporting Evidence

Evidence to include where available and appropriate:

- GitHub commits demonstrating development changes.
- Screenshots of the GuardPulse storefront and relevant functionality.
- Backend code and test results supporting claims about implementation and testing.
- Evidence of shipping-rate integration and the current payment sandbox status.

All evidence should reflect work actually completed and must not expose credentials, secrets, customer data, or other confidential information.
