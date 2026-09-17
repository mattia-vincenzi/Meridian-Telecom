# Platform Engineer - Final Take-Home Assignment

## Context - Meridian Telecom

Meridian Telecom is a fictional mobile operator building an internet-facing service where customers can purchase and manage mobile subscriptions through an AI-powered chatbot.

A customer can ask about plans, choose an offer, provide their details, complete an identity check, pay, and request a physical SIM delivered to their address. The platform should coordinate the process automatically and keep the customer informed until the SIM is delivered and the service is activated.

The journey is not always completed in one conversation. A customer may leave and return later, provide missing identity documents, correct delivery details, or ask why their payment or activation is still pending. Some cases require manual review. Delivery and activation may take several days, and exceptional cases may remain open for weeks.

Customers expect quick chatbot responses even when many others are signing up. They should be able to resume their journey and check its status without starting again; progress and pending actions must survive disconnections, restarts and deployments. Incorrect or repeated actions must not cause duplicate charges, duplicate SIM shipments or activation before the required checks have passed.

Identity verification, payments, SIM fulfilment and telecom provisioning are provided by existing systems or external providers with APIs. AI Engineers develop the conversational agents and business logic. Your responsibility is the platform infrastructure supporting this customer journey and its operation at scale.

Most work is I/O-bound, with some CPU-intensive document or audio processing. Selected models may run on company-managed GPUs, while external AI providers impose rate limits and charge for usage. Identity verification itself is an existing integration.

The launch expects approximately 100 users and a modest workload. The platform should start economically, with a credible path to 100,000 users, thousands of concurrent chatbot sessions and hundreds of thousands of background tasks per day, without a fundamental redesign.

## Technical context and constraints

AWS is the cloud provider, and Kubernetes is the target runtime. The first production environment will use managed Kubernetes on AWS. Meridian Telecom wants to avoid unnecessary provider lock-in, while using managed services where the benefits justify the dependency.

The platform is maintained by two Platform Engineers, working alongside AI Engineers. The Platform team owns infrastructure, its operating costs and operability. AI Engineers primarily own agent behaviour, orchestration logic, and model usage and costs; consider the interface between these responsibilities.

Assume that:

- the service is exposed on the public internet;
- agent runs and external actions must be traceable and auditable;
- confidential customer data must remain in the selected region;
- the availability objective is 99.9%;
- conversation and durable workflow state require an RPO below one minute and an RTO below ten minutes;
- infrastructure spending must be measurable and sustainable as usage grows.

## Your task

Design the platform and explain the decisions behind your proposed solution. The primary focus is infrastructure and platform engineering, with a strong system and software design component.

Identify what deserves attention and consider the trade-offs across technology choices, scalability, reliability, security, observability, infrastructure cost and operational complexity. Explain how the solution can be built, validated and operated by the available team, including your development approach, indicative delivery timeline and priorities from launch through later growth.

Make reasonable assumptions and highlight the uncertainties that materially affect your decisions. We value a coherent, well-explained proposal and clear prioritisation.

## Preparation and use of AI

We recommend spending two to three hours on preparation. This is not a strict maximum: solving the full problem for production could take days or weeks. Choose the level of detail that best communicates your thinking within the suggested time. No working implementation or demo is required.

Use Claude Code, Codex, or another AI agent to help prepare your solution. You remain responsible for the decisions. Briefly describe the tools and models used, what you delegated, any suggestions you accepted, rejected or substantially changed, and how you reviewed and validated the work. A complete chat transcript is not required. Do not incur additional cloud or model costs for this exercise.

## Deliverable and discussion

Prepare material for an approximately 30-minute presentation, followed by technical discussion. Use any format that helps you show the infrastructure, solution and decisions: slides, diagrams, a PDF, a custom HTML presentation, or another useful format. Supporting artifacts are optional.

The complete in-person meeting will last approximately two to three hours, including time to meet the team and speak with HR.
