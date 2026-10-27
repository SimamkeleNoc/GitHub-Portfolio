# Sprint Backlog — GuardPulse

## 1. Purpose

The sprint backlog identifies a focused set of tasks that could be completed during one development iteration. It connects the broader GuardPulse product backlog to a practical development goal.

**Documentation note:** This is a proposed sprint plan created for the PRP370S portfolio. It is not a historical sprint record. The tasks must be carried out and verified before they can be marked complete.

## 2. Sprint Goal

**Proposed goal:** Improve confidence in the GuardPulse checkout journey by reviewing cart calculations, stock handling, delivery-rate responses, and payment sandbox behaviour.

This goal focuses on reliability in the purchasing process while recognising that PayFast is still in sandbox mode.

## 3. Selected Tasks

| Task ID | Task | Priority | Evidence required |
|---|---|---|---|
| SB01 | Review cart totals and checkout input validation | High | Relevant code review and test results |
| SB02 | Verify stock handling during checkout | High | Automated test results and any identified defects |
| SB03 | Check delivery-rate integration and error handling | High | Test results or screenshots of rate responses |
| SB04 | Verify supported PayFast sandbox outcomes | High | Sandbox test evidence with credentials removed |
| SB05 | Record defects and create follow-up backlog items | Medium | Documented findings and prioritised follow-up tasks |

## 4. Acceptance Criteria

The proposed iteration will be considered successful when:

- Cart totals and required checkout inputs have been reviewed and relevant tests have been run.
- Stock-related behaviour has been checked against the expected application rules.
- Delivery-rate responses and unsuccessful requests have been examined.
- Supported payment sandbox outcomes have been verified without exposing sensitive configuration.
- Any defects or incomplete work have been recorded for follow-up.

These criteria describe the intended outcome. They do not mean the tasks have already passed testing.

## 5. Work Tracking

For this proposed iteration, tasks can be tracked using the following statuses:

- **To do:** Work has not yet started.
- **In progress:** Work is currently being investigated or implemented.
- **Blocked:** Work depends on an unresolved issue or external requirement.
- **Done:** The task has been completed and supporting evidence has been checked.

Git and GitHub commits can be used to trace code changes. Test results and screenshots can provide additional evidence of behaviour.

## 6. Dependencies and Risks

- PayFast account verification is pending, so real payments are not enabled.
- External shipping-rate services may return errors or unavailable rates.
- Changes to checkout or stock handling may affect related functionality.
- The backend rewrite from Java and Spring Boot to TypeScript and Hono makes regression testing important.

Any dependency that prevents a task from being completed should be documented rather than reported as a successful result.

## 7. Review and Reflection

This proposed sprint demonstrates how a broad product backlog can be narrowed into a focused set of tasks with a shared goal. Concentrating on checkout reliability helps connect technical work to the customer experience.

Working independently means I must manage task selection, implementation, testing, and follow-up myself. A structured sprint backlog would help me make priorities explicit and identify blockers earlier. In future development, I would record task status and testing evidence as work progresses, then review the results at the end of the iteration.

## 8. Evidence to Collect

- Relevant checkout and cart tests.
- Stock-handling test results.
- Delivery-rate integration evidence.
- PayFast sandbox test evidence.
- GitHub commits related to completed work.
- A list of defects, limitations, and follow-up tasks.

Only mark a task as done after checking the implementation and its supporting evidence.
