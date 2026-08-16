# GS-WEB-005 Update Design System

## Status: To Be Implemented

**Parent Issue:** GS-WEB-004 (Architecture Team Delivery Docket)

**Author:** Morpheus (Delivery Architect)

---

## Objective

Update the website's SCSS colour system to match the approved design specification (GS-WEB-003).

Currently, the website uses **purple (#7c3cff)** and **cyan (#00f5ff)** accents, which contradict the approved **green** colour system.

---

## Current State (VIOLATION)

| Element | Current Value | Approved Value |
|---------|---------------|----------------|
| Primary Accent | #7c3cff (Purple) | #4CAF6A (Green) |
| Secondary Accent | #00f5ff (Cyan) | #95E5B1 |
| Background Primary | #04030a | #060807 |
| Background Secondary | - | #0D1311 |
| Background Surface | - | #131B18 |
| Text Primary | #e8f7ff | #EDF2EF |
| Text Secondary | #8fa8c4 | #C9D4CD |

---

## Required Changes

### 1. Update SCSS Variables

Replace all accent colour references in `assets/css/style.scss`:

```scss
// Change from:
$accent: #7c3cff;
$accent-2: #00f5ff;

// Change to:
$accent: #4CAF6A;
$accent-2: #95E5B1;
```

### 2. Update Gradient Overlays

Replace all purple/cyan gradient overlays with approved green palette.

### 3. Update Interactive States

Update all button, hover, and emphasis states to use green accents.

### 4. Update Selection Colour

Update `::selection` colour to match green theme.

---

## Acceptance Criteria

- [ ] Primary accent is green (#4CAF6A)
- [ ] Secondary accent is #95E5B1
- [ ] No purple (#7c3cff) or cyan (#00f5ff) visible
- [ ] All gradients use approved colours
- [ ] Interactive states use green accents
- [ ] WCAG AA contrast ratios maintained
- [ ] Visual review confirms brand identity

---

## Dependencies

- GS-WEB-004 (Delivery Planning) - APPROVED
- GS-WEB-003 (Design Guide) - Authoritative

---

## Notes

This is a **CRITICAL** change. The current purple/cyan design creates a "cyberpunk" and "tech startup" aesthetic that contradicts the approved "natural, grounded, green" identity.

All colour changes must be verified against GS-WEB-003 before proceeding to content updates.

---

**[End of Issue]**