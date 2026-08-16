# GS-WEB-008 Update Navigation

## Status: To Be Implemented

**Parent Issue:** GS-WEB-004 (Architecture Team Delivery Docket)

**Author:** Morpheus (Delivery Architect)

---

## Objective

Update the website navigation to include all 5 pages as specified in GS-WEB-001 (Architecture Specification).

**Current Navigation:**
- Home
- About
- Contact

**Approved Navigation (GS-WEB-001, section 9):**
- Home
- About
- Philosophy
- Approach
- Contact

---

## Current State (VIOLATION)

### Layout (default.html)

```html
<nav class="main-nav">
  <ul>
    <li><a href="/">Home</a></li>
    <li><a href="/about">About</a></li>
    <li><a href="/contact">Contact</a></li>
  </ul>
</nav>
```

**Missing:** Philosophy and Approach links

### Navigation Order Violation

GS-WEB-001 (architecture.md, section 9) specifies the exact navigation order:

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

Current order does not match approved sequence.

---

## Required Changes

### 1. Update Navigation Links

Replace the navigation in `_layouts/default.html`:

```html
<nav class="main-nav">
  <ul>
    <li><a href="/">Home</a></li>
    <li><a href="/about">About</a></li>
    <li><a href="/philosophy">Philosophy</a></li>
    <li><a href="/approach">Approach</a></li>
    <li><a href="/contact">Contact</a></li>
  </ul>
</nav>
```

### 2. Update Active State Logic

Ensure active state logic correctly highlights current page:

```html
<li><a href="/" {% if page.url == "/" %}class="active"{% endif %}>Home</a></li>
<li><a href="/about" {% if page.url == "/about" %}class="active"{% endif %}>About</a></li>
<li><a href="/philosophy" {% if page.url == "/philosophy" %}class="active"{% endif %}>Philosophy</a></li>
<li><a href="/approach" {% if page.url == "/approach" %}class="active"{% endif %}>Approach</a></li>
<li><a href="/contact" {% if page.url == "/contact" %}class="active"{% endif %}>Contact</a></li>
```

### 3. Mobile Navigation

Ensure mobile menu includes all 5 links:

- Collapse into mobile menu on small screens
- All links accessible
- Touch-friendly spacing

---

## Acceptance Criteria

- [ ] Navigation includes all 5 links
- [ ] Link order matches GS-WEB-001 (section 9)
- [ ] Active state logic works correctly
- [ ] Mobile navigation includes all links
- [ ] Links point to correct pages
- [ ] No broken links
- [ ] Navigation visible on all pages

---

## Dependencies

- GS-WEB-004 (Delivery Planning) - APPROVED
- GS-WEB-001 (Architecture) - Authoritative (navigation order)
- GS-WEB-005 (Design System Update) - Should be completed first
- GS-WEB-006 (Content Updates) - Should be completed first
- GS-WEB-007 (Create Missing Pages) - Must be completed first

---

## Notes

### Implementation Order

**This should be done AFTER:**
1. GS-WEB-005 (Design System) - Colours updated
2. GS-WEB-006 (Content Updates) - Content updated
3. GS-WEB-007 (Create Missing Pages) - Pages exist

**Reason:** Links will be broken until pages exist and content is ready.

### User Journey

The navigation order is designed to guide visitors through:

1. **Identity** (Home, About)
2. **Worldview** (Philosophy)
3. **Methodology** (Approach)
4. **Engagement** (Contact)

This progression must be preserved.

---

## Footer Update

Also update footer navigation (if present) to match the same order:

```
Home → About → Philosophy → Approach → Contact
```

---

**[End of Issue]**