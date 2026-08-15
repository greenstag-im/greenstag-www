# Green Stag Public Website - Architecture Specification

Status: Approved Baseline
Version: 1.0
Author: Cody

Repository:
greenstag_www

Location:
/docs/website/architecture.md

---

## 1. Architectural Purpose

This document defines the public website architecture for Green Stag.

The purpose of this document is to create a durable architectural baseline that can be consumed by:

- Content authors
- Designers
- Implementation workers
- Reviewers

without requiring access to internal strategy documents.

This document is the authoritative source for:

- Website structure
- Website purpose
- Information architecture
- Page relationships
- User journeys
- Navigation architecture
- Future expansion architecture

This document is not responsible for:

- Page copy
- Visual design
- Styling
- Implementation details

---

## 2. Website Mission

The website exists to communicate:

- Purpose
- Philosophy
- Worldview
- Approach

The website does not exist primarily to:

- Sell products
- Market services
- Generate leads
- Promote unreleased initiatives

Success is measured by:

Visitor Understanding

rather than

Visitor Conversion

---

## 3. Architectural Principles

All future website decisions should align with the following principles.

## Understanding Before Promotion

Visitors should understand Green Stag before being asked to engage.

## Philosophy Before Products

The organisation's beliefs are more important than its current offerings.

## Curiosity Before Certainty

The website should encourage exploration and thought.

## Clarity Before Complexity

Complex ideas should be communicated clearly.

## Foundations Before Expansion

The architecture should support future growth without redesign.

## Long-Term Thinking

The website should remain relevant as the organisation evolves.

---

## 4. Audience Model

Primary Audience

- Curious visitors
- Potential collaborators
- Industry peers
- Technologists
- Researchers

Secondary Audience

- Future customers
- Future contributors
- Journalists
- Students

The website is intentionally not optimised for:

- Sales funnels
- High-pressure marketing
- Conversion campaigns

---

## 5. Site Architecture

Version 1 contains five pages.

/

Home

/about

About Green Stag

/philosophy

The Green Stag Philosophy

/approach

How Green Stag Thinks

/contact

Start A Conversation

No additional pages exist in Version 1.

---

## 6. Information Hierarchy

The website hierarchy is intentional.

### Tier 1

Home

Philosophy

These pages define identity and purpose.

---

### Tier 2

Approach

About

These pages provide supporting context.

---

### Tier 3

Contact

This page enables engagement.

---

## 7. Page Relationship Model

Each page has a specific responsibility.

### Home

Introduces Green Stag.

Creates curiosity.

Encourages exploration.

---

### About

Explains organisational identity.

Explains why Green Stag exists.

---

### Philosophy

Defines beliefs.

Defines worldview.

Defines purpose.

This is the conceptual centre of the website.

---

### Approach

Explains methodology.

Explains thinking.

Explains how Green Stag approaches problems.

---

### Contact

Enables communication.

Provides a path for engagement.

---

## 8. User Journey Architecture

### Primary Journey

Home

↓

Philosophy

↓

Approach

↓

Contact

Purpose:

Move a visitor from curiosity to understanding to engagement.

---

### Secondary Journey

Home

↓

About

↓

Philosophy

Purpose:

Move a visitor from identity to worldview.

---

### Independent Journey

Any Page

↓

Philosophy

Purpose:

Ensure every visitor can discover Green Stag's core beliefs.

---

## 9. Navigation Intent

Navigation order is deliberate.

Home

↓

About

↓

Philosophy

↓

Approach

↓

Contact

The sequence moves visitors through:

Identity

↓

Worldview

↓

Methodology

↓

Engagement

Future navigation changes should preserve this progression.

---

## 10. Home Architecture

Purpose:

Introduction

Required Outcomes:

Visitor understands:

- Green Stag exists
- Green Stag has a philosophy
- Green Stag is worth exploring

Required Sections:

Hero

Mission Statement

Core Principles

Approach Summary

Call To Action

---

## 11. About Architecture

Purpose:

Identity

Required Outcomes:

Visitor understands:

- Who Green Stag is
- Why Green Stag exists

Required Sections:

Who We Are

Why We Exist

Future We Want To Help Build

Leave Things Better Than You Found Them

---

## 12. Philosophy Architecture

Purpose:

Worldview

Required Outcomes:

Visitor understands:

- Core beliefs
- Core values
- Purpose

Required Sections:

Why We Are Here

Shine A Light

Question Assumptions

Build Better Systems

Remain Curious

The Caretaker's Charge

This page is considered the most important page after Home.

---

## 13. Approach Architecture

Purpose:

Methodology

Required Outcomes:

Visitor understands:

- How Green Stag thinks
- How Green Stag approaches complexity

Required Sections:

Systems Thinking

Architecture Before Scale

Governance By Design

Human And Machine Collaboration

Knowledge As An Asset

Continuous Improvement

---

## 14. Contact Architecture

Purpose:

Engagement

Required Outcomes:

Visitor understands how to contact Green Stag.

Required Sections:

Introduction

Contact Information

Call To Action

---

## 15. Content Domains

Future content must belong to one of the following domains.

Identity

Philosophy

Approach

Products

Research

Resources

New content outside these domains requires architectural review.

---

## 16. Future Expansion Architecture

Reserved Locations:

/products

/projects

/research

/resources

/articles

No placeholder pages should exist.

No "coming soon" pages should exist.

Future pages should be added only when meaningful content exists.

---

## 17. Content Boundaries

Approved Topics:

- Curiosity
- Understanding
- Systems
- Architecture
- Governance
- Learning
- Stewardship
- Better Futures

Avoid:

- Internal structures
- Confidential planning
- Proprietary implementation details
- Unreleased initiatives

When uncertain:

Prefer omission.

---

## 18. Ownership Model

Architecture owns:

- Site structure
- Site purpose
- Information architecture
- Page responsibilities

Content owns:

- Copy
- Messaging
- CTA language

Design owns:

- Visual language
- Components
- Styling

Implementation owns:

- HTML
- SCSS
- Jekyll implementation

---

## 19. Technical Architecture

Platform:

Jekyll

Hosting:

GitHub Pages

Content:

Markdown

Styling:

SCSS

Requirements:

- Static deployment
- Mobile responsive
- Accessible
- Fast loading
- Minimal JavaScript

No requirement exists for:

- CMS
- Database
- Dynamic backend

---

## 20. Repository Architecture

Authoritative Files

/docs/website/architecture.md

/docs/website/content.md

/docs/website/design.md

Workers should treat these files as authoritative.

Issues describe work.

Repository documents describe truth.

---

## 21. Acceptance Criteria

GS-WEB-001 is complete when:

✓ Site structure defined

✓ User journeys defined

✓ Information hierarchy defined

✓ Page relationships defined

✓ Navigation intent defined

✓ Future expansion architecture defined

✓ Content boundaries defined

✓ Ownership model defined

✓ Technical architecture defined

✓ Repository architecture defined

GS-WEB-002 must be executable using this document alone.

GS-WEB-003 must be executable using this document and GS-WEB-002.

Implementation workers must be able to understand the website architecture without access to internal notebooks.

---

## Architectural Decision

Version 1 of the Green Stag website prioritises identity, philosophy and understanding over products, services or promotion.

The website exists to help visitors understand why Green Stag exists before asking them to engage with what Green Stag does.
