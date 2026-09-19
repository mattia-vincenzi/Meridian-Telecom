# Meridian Telecom — Platform Engineer Take-Home

Design proposal and presentation material for an AI-powered mobile subscription platform, covering the customer journey from plan selection to SIM delivery and activation.

The proposed architecture combines AWS EKS, RDS PostgreSQL, Step Functions, SQS and S3 to keep conversations responsive and long-running workflows recoverable. The material discusses safe external actions, reliability, security, scaling, costs and delivery priorities for a two-person Platform team.

- [Assignment](assignment.md) — authoritative requirements and constraints.
- [Original assignment](original/Platform_Take_Home_Assignment.pdf) — assignment supplied as a PDF.
- [Solution](solution.md) — proposed architecture, trade-offs, assumptions, costs, delivery roadmap and AI usage notes.
- [Presentation deck](presentation/meridian_mattia_vincenzi.pptx) — PowerPoint material for the technical discussion.
- [Architecture diagram](img/architecture.png) — platform architecture image.
- [Network diagram](img/schema_rete.png) — network layout image.
- [Failure example](diagrams/failure_example_mermaid.txt) — Mermaid source for the payment recovery sequence.
- [AI working instructions](AGENTS.md) — repository guidelines for AI-assisted preparation.
- [Ignore rules](.gitignore) — files excluded from version control.
