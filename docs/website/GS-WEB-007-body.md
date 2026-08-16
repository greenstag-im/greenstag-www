# GS-WEB-007 Create Missing Pages - Philosophy and Approach

## Status: To Be Implemented

**Parent Issue:** GS-WEB-004 (Architecture Team Delivery Docket)

**Author:** Morpheus (Delivery Architect)

---

## Objective

Create two critical pages that are currently **missing** from the website:

1. **Philosophy** (philosophy.md) - The intellectual centre of the website
2. **Approach** (approach.md) - Explains how Green Stag thinks

These pages are **REQUIRED** per GS-WEB-001 (Architecture Specification).

---

## Architecture Requirements (GS-WEB-001)

### Page Hierarchy

| Tier | Pages |
|------|-------|
| **Tier 1** | Home, Philosophy |
| **Tier 2** | Approach, About |
| **Tier 3** | Contact |

**Note:** Philosophy is explicitly stated as "the most important page after Home" (architecture.md, section 12).

### Approved Navigation (architecture.md, section 9)

```
Home
↓
About
↓
Philosophy
↓
Approach
↓
Contact
```

**Current State:** Philosophy and Approach links are **MISSING**.

---

## Content Source

Both pages must use content from **GS-WEB-002 (Content Baseline)**:

### Philosophy Page Content

**Required Sections (GS-WEB-002):**

1. Why We Are Here
2. Shine A Light
3. Question Assumptions
4. Build Better Systems
5. Remain Curious
6. The Caretaker's Charge
7. Closing Reflection
8. CTA: "Explore How We Think" → Approach

**Page Structure (GS-WEB-003, section 67):**

```
Navigation
↓
Page Header
↓
Why We Are Here
↓
Shine A Light
↓
Quote Block
↓
Question Assumptions
↓
Build Better Systems
↓
Remain Curious
↓
The Caretaker's Charge
↓
Closing Reflection
↓
CTA
↓
Footer
```

### Approach Page Content

**Required Sections (GS-WEB-002):**

1. Systems Thinking
2. Architecture Before Scale
3. Governance By Design
4. Human And Machine Collaboration
5. Knowledge As An Asset
6. Continuous Improvement
7. Closing Reflection
8. CTA: "Start A Conversation" → Contact

**Page Structure (GS-WEB-003, section 68):**

```
Navigation
↓
Page Header
↓
Systems Thinking
↓
Architecture Before Scale
↓
Governance By Design
↓
Human And Machine Collaboration
↓
Knowledge As An Asset
↓
Continuous Improvement
↓
Closing Reflection
↓
CTA
↓
Footer
```

---

## Implementation Requirements

### 1. Page Structure

- Use Jekyll layout: `layout: default`
- Include page header component
- Use long-form content component
- Include closing reflection
- Add CTA section
- Link to next page in journey

### 2. Navigation Updates

After creating pages, update `_layouts/default.html`:

- Add "Philosophy" link
- Add "Approach" link
- Update active state logic

### 3. Mobile Responsive

- Single column layout
- Typography scaled for mobile
- No horizontal scrolling
- Readable without zoom

### 4. Accessibility

- WCAG AA contrast
- Keyboard accessible
- Semantic HTML
- Alt text for images

---

## Acceptance Criteria

- [ ] philosophy.md created with approved content
- [ ] approach.md created with approved content
- [ ] Both pages use GS-WEB-002 content exactly
- [ ] Both pages use GS-WEB-003 design system
- [ ] Navigation includes new links
- [ ] Mobile responsive tested
- [ ] Accessibility verified
- [ ] Links between pages follow user journey

---

## Dependencies

- GS-WEB-004 (Delivery Planning) - APPROVED
- GS-WEB-002 (Content Baseline) - Authoritative
- GS-WEB-003 (Design Guide) - Authoritative
- GS-WEB-005 (Design System Update) - Should be completed first
- GS-WEB-006 (Content Updates) - Related, may be combined

---

## Notes

### Priority

**HIGH PRIORITY** - These pages are critical for completing the approved user journey.

### Architecture Priority

Per GS-WEB-001 (architecture.md, section 12):

> "This page [Philosophy] is considered the most important page after Home."

### Content Priority

These pages must use **exact** content from GS-WEB-002. No modifications allowed.

---

**[End of Issue]**