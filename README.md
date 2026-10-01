# ArcanoZero

## Case Study

ArcanoZero is a private restaurant commerce project designed around configurable branding and a progressive path from first party ordering to broader operational capabilities.

This repository is a portfolio case study. It does not contain the private source code or the internal technical documentation required to reproduce the product.

## The Problem

Restaurants often depend on external platforms for customer relationships, ordering and operational data.

ArcanoZero explores how a restaurant can progressively own more of its digital commerce experience while keeping the software architecture adaptable to future integrations.

The engineering challenge is to build useful commerce capabilities now without prematurely coupling the system to payment providers, logistics providers, ERP platforms or infrastructure that has not yet been justified.

## My Role

I direct the product and engineering process with AI coding agents acting as implementation collaborators.

My responsibilities include:

* Product definition
* Architecture decisions
* Domain modeling
* Technical specifications
* Agent orchestration
* Acceptance criteria
* Review and validation
* Security boundaries
* Progressive delivery decisions

The project demonstrates an AI directed development workflow applied to conventional product software.

## Current Product Foundation

The private implementation currently includes working foundations for:

* Catalog data
* Address validation and serviceability
* Persistent carts
* Server side pricing behavior
* Versioned REST APIs
* Runtime input validation
* Revision controlled mutations
* Order creation
* Idempotent operations
* Immutable order snapshots
* Guest access boundaries
* PostgreSQL persistence
* Configurable branding

Some user interface areas remain intentionally incomplete or presentation only.

Payment settlement, production logistics integrations, ERP integrations and authenticated operational workflows are not represented as completed capabilities.

## Engineering Approach

A simplified public representation of the current commerce flow is:

```text
Catalog
   |
   v
Cart
   |
   v
Server Validation
   |
   v
Pricing
   |
   v
Place Order
   |
   v
Idempotency
   |
   v
Immutable Order Snapshot
```

The private implementation contains additional constraints, persistence rules and security details that are intentionally not reproduced here.

## What This Project Demonstrates

### Product Engineering

Business requirements are translated into domain concepts, server behavior, persistence and user facing flows.

### Domain Modeling

Commerce concepts such as catalog, cart, pricing and order state are represented explicitly rather than being scattered across interface code.

### API Design

Server capabilities are exposed through versioned APIs with runtime validation and controlled error behavior.

### PostgreSQL Modeling

Persistence includes relational constraints and state consistency rules, while sensitive implementation details remain private.

### Idempotency

Retry sensitive mutations are designed so repeated requests do not silently create duplicated business effects.

### Security Boundaries

The browser is treated as an untrusted client. Authoritative business behavior remains server side.

### White Label Foundation

Customer facing identity is configuration driven so a deployment does not require scattered brand hardcoding.

### Agent Directed Development

AI coding agents perform implementation work under explicit architecture, scope constraints and acceptance criteria.

## Architecture Direction

The project follows a modular architecture with explicit domain boundaries and provider isolation.

External integrations are intended to remain behind stable boundaries so that payment, logistics and operational providers do not become the internal domain model.

Only the architectural principle is presented here. Internal interfaces and integration designs remain private.

## Technology Areas

The private implementation currently includes work across:

* TypeScript
* React
* TanStack
* PostgreSQL
* SQL migrations
* REST APIs
* Zod
* Bun
* Automated testing
* Domain modeling
* Runtime validation
* Idempotent server workflows
* Configurable branding

This list describes demonstrated engineering areas, not the full private repository.

## Current Boundaries

ArcanoZero is an active development project.

The public case should not be interpreted as evidence of:

* Production payment processing
* Live payment settlement
* Production logistics integrations
* ERP or POS integration
* Owned courier fleet
* Shared database SaaS multi tenancy
* Production scale traffic
* Completed customer authentication
* Fully completed operational tooling

## Why This Case Is Public

The goal of this repository is to demonstrate product and engineering capability without publishing the implementation required to clone the product.

Source code, provider designs, internal specifications, database details beyond high level descriptions, credentials and proprietary operational logic remain private.

## Portfolio Context

ArcanoZero demonstrates conventional product engineering performed through an AI directed workflow.

For a complementary example focused on LLM applications, evaluation and deterministic AI boundaries, see the Pulso case study in my GitHub profile.
