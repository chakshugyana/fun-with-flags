# ADR-001: Repository Strategy

- **Status:** Accepted
- **Date:** 2026-10-11

## Context

BankingApp is a learning capstone covering Java, Spring Boot, Kafka, IBM ACE, React Micro Frontends, databases, and automated testing.

Two repositories already exist:

- `fun-with-flags`
- `ace-the-race`

The project needs clear ownership boundaries without duplicating implementations or making local development unnecessarily difficult.

## Decision

Retain the two existing repositories.

- `fun-with-flags` will host Spring Boot, Java, Kafka, and backend learning exercises.
- `ace-the-race` will host IBM ACE integration flows, ACE-specific artifacts, and integration learning documentation.

The repositories will collaborate through documented API contracts, event schemas, and integration specifications.

The React repository placement will be decided when the frontend module is planned.

## Consequences

### Positive

- Each repository has a clear learning focus.
- ACE-specific and Java-specific development can progress independently.
- Existing work is preserved.

### Trade-offs

- Cross-repository changes require coordination.
- Integration tests must run against compatible versions of both projects.
- API and event contracts must remain synchronized.

## Revisit When

The number of components, deployment requirements, or team ownership model makes a different repository structure more appropriate.
