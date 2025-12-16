![In Review](https://img.shields.io/badge/Phase-review-amber)

# Quality Engineering: building, testing and assuring quality across your service

## Why this matters

Quality engineering is how you build confidence that your service works for users, stays reliable, and can change safely at pace. It is a broader approach that builds on quality assurance, but extends it across the whole service lifecycle, from design and development to live operations and continuous improvement. Quality engineering brings together assurance, testing, verification, validation, monitoring, reliability and resilience into one continuous system. It reflects how modern digital teams work: designing for quality, testing early and often, establishing a continuous feedback loop, monitoring outcomes and improving.

It’s about engineering the quality in, not checking it at the end.

## Quality is a shared responsibility

Everyone is responsible for the quality of what they deliver. That means:

- understanding what quality means for your users and service
- designing for testability, reliability, accessibility, and security
- testing early and often
- monitoring how the service behaves in live
- improving based on what you learn

Quality assurance is a team effort supported by specialist skills. Different types of expertise help make this possible, from testing, evaluation and automation to performance, resilience, and operational readiness assessment. Adopt software engineering practices like test-driven development (TDD) or pair programming to embed testing early.

## Design for quality from the start

Plan how you’ll build and test quality starting from discovery and alpha, not after you’ve built something. Designing for testability and resilience reduces risk later.

Do this by:

- identifying the risks and how you’ll manage them
- designing systems that are easy to test and observe
- analysing risks, constraints and assumptions that might affect quality
- validating assumptions through prototypes or experiments
- agreeing early definitions of quality for the service and users
- building environments that reflect live conditions
- automating checks that give fast feedback
- protecting user data through safe, synthetic test data or masking
- thinking about recovery, resilience, and support from day one

## Test and learn continuously

Testing isn’t a one-off activity. It’s how you learn whether your service behaves as expected and how you build evidence that it’s ready for users. Quality engineering works well in short and continuous feedback loops: Discover, Plan, Build, Observe, Learn. At each stage:

- test what you’ve built under normal and unusual conditions
- observe how it behaves in different environments and devices
- learn from data, incidents, and user feedback
- feed those lessons into test design and delivery decisions
- adopt an in sprint automation approach where possible
- test the changes in automated way for continuous deployments

Testing and learning continuously help you release safely and confidently. Adopt a risk-based test pyramid. Set a flake budget and track test stability. Any production defect should result in a new automated regression test.

Keep testing in pipelines fast by using:

- parallelise
- ephemeral environments
- deterministic test data
- contract/API tests over end-to-end UI where possible.

Design tests based on risks covering product factors, user journeys, data, interfaces, time, and quality criteria categories (capability, usability, security, reliability, etc.).

## Use a holistic assurance approach

Combine automation, exploration, and expert judgement. Each plays a role in testing and assuring quality. Automated checks give fast feedback and guard against regression. Exploratory testing helps uncover risks that tools can’t see. Verification and validation provide confidence that your service does what it should, for the people it’s meant to serve.

You should also test for:

- performance and scalability - will it stay fast and stable as demand grows?
- security and privacy - does it protect users and data?
- accessibility and inclusion - does it work for everyone, including disabled users?
- resilience and recovery - how does it behave when things fail?
- functional testing - can it do what it’s coded to do?
- compatibility - does it work for supported browsers, OS versions and devices?

Quality engineering brings these threads together into a single picture of confidence. For services with APIs or microservices, implement contract tests that run on every pull request and in CI. Map risks to test types: contracts for integration risk, chaos/failover tests for resilience, targeted performance tests for peak journeys, and pen testing for exposed surfaces.

## Keep monitoring in live

Assurance doesn’t stop at release. Your service should:

- release gradually using feature flags or canary or blue/green deployments
- track Service Level Objectives (SLOs) and error budgets for performance and reliability
- use monitoring, alerting and analytics to understand live behaviour
- rehearse incident response and recovery
- review incidents openly and turn findings into improvements

Build your observability and resilience practices alongside your testing, they’re both part of assurance.

## Testing AI-enabled services

If your service includes data AI, you’ll need additional testing and assurance steps. You should check for:

- bias or unfair outcomes
- accuracy and reliability of results
- explainability — can you understand why it produced an answer?
- drift over time as data or context changes
- ethical and legal compliance

Please refer to the [xGov AI testing framework](https://testing-ai-standards.github.io/cross-gov-ai-testing-framework/) for a detailed understanding of quality attributes and more prescriptive insights on incorporating a defensive delivery model for AI systems.

## Measure quality and reliability

Use a few meaningful and measurable metrics to understand how well your service meets its quality goals. For example:

- DORA metrics for delivery performance
- SLO attainment for performance and availability
- accessibility score
- test stability (flake rate)
- Defect detection efficiency
- security vulnerabilities and fix times

## Evaluate operational readiness

Before releasing or scaling your service, make sure it’s operationally ready. You should have:

- automated deployment and rollback
- tested backup, recovery and failover
- clear runbooks and alerts
- monitoring and observability aligned to your SLOs
- agreed support arrangements and on-call capability
- confidence that known risks are documented and understood

Operational readiness is part of assurance,  it proves the service can perform and recover in the real world.

## Human side of quality

Quality is a socio-technical outcome, it depends on the people, the systems they build, and how they work together. Testing and assurance are cognitive activities. They need curiosity, critical thinking and collaboration as much as tools and automation.

Teams should invest in developing:

- exploratory skills - learning through investigation, observation and questioning
- heuristics and problem-solving - using experience and structured thinking to test what matters most
- communication - sharing evidence clearly so teams can make informed decisions
- systems thinking - seeing how business, technology, policy, operations and users connect
- empathy - understanding users, colleagues and the impact of failure

A strong culture of learning supports these skills. Create space for pairing, peer reviews, retrospectives and knowledge-sharing.

## Keep improving your testing approach

Quality engineering evolves as technology and risks change. Keep improving by:

- reviewing incidents and live data regularly
- updating your test and assurance strategy
- experimenting with new tools and techniques
- sharing lessons with other teams and communities across government

Operate to SLOs and error budgets. After incidents, add regression tests by default and retire flaky or low-value tests. Publish a monthly quality scorecard where possible.

Building reliable, resilient services depends on how well teams learn and adapt together.
