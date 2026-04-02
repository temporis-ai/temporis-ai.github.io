# Temporis Website Implementation Plan

## 1. Purpose
This document translates [design.md](design.md) into an implementation plan for the current repository.

It defines:

- page and file structure
- build order
- component mapping
- content and asset requirements
- accessibility, SEO, and performance requirements
- launch criteria for each phase

The site remains a static website for v1.

Responsive behavior on both desktop and mobile is a required part of v1, not a follow-up task.

### Domain and launch model
- `temporis.co` and `www.temporis.co` host the company website.
- Vista and Platform will eventually live on:
  - `vista.temporis.co`
  - `platform.temporis.co`
- those product subdomains are not live yet.
- for launch, product pages should live on the main company site as:
  - `/vista`
  - `/platform`

These are public product overview pages that can later redirect to the subdomains.

### Simplified IA rule
The top-level site structure should stay at:
- Products
- Company
- Contact

Do not expose internal model terminology as a top-level navigation requirement for first-time visitors.

## 2. Current Repo Assessment
Current repo files:

- [index.html](../index.html)
- [about.html](../about.html)
- [contact.html](../contact.html)
- [styles.css](../styles.css)

Current issues relative to the design:

- `about.html` and `contact.html` likely need content and layout rewrites.
- `index.html` uses consulting-style messaging and must be rebuilt.
- `styles.css` is a generic single-theme stylesheet and should be replaced with a more deliberate system.
- required pages for `Vista`, `Platform`, and legal documents do not yet exist.

## 3. Target File Structure

### Keep
- [index.html](../index.html)
- [contact.html](../contact.html)
- [styles.css](../styles.css)

### Rewrite / repurpose
- [about.html](../about.html) -> company page content

### Create
- `vista.html`
- `platform.html`
- `privacy.html`
- `terms.html`
- `disclaimer.html`
- optional shared assets folder later if screenshots or diagrams are added

### Recommended v1 routing
- `/` -> `index.html`
- `/vista` -> `vista.html`
- `/platform` -> `platform.html`
- `/company` -> `about.html`
- `/contact` -> `contact.html`
- `/privacy` -> `privacy.html`
- `/terms` -> `terms.html`
- `/disclaimer` -> `disclaimer.html`

### Future routing plan
- when `vista.temporis.co` is ready, `/vista` can redirect there
- when `platform.temporis.co` is ready, `/platform` can redirect there
- the product pages should remain the canonical explanation layer until those destinations are live

## 4. Build Strategy
Build the site in layers, not page by page in isolation.

### Layer 1: global system
- typography
- color tokens
- spacing scale
- layout containers
- buttons
- nav
- footer
- card system
- screenshot frame
- code block
- disclosure block

### Layer 2: homepage
- hero
- why Temporis
- Vista / Platform split
- company / research section
- trust section
- final CTA

### Layer 3: product pages
- Vista
- Platform

### Layer 4: supporting pages
- Company
- Contact
- Legal pages

This avoids rebuilding the same design decisions multiple times.

## 5. Page-to-File Mapping

### Home
File:
- [index.html](../index.html)

Required sections:
- sticky header
- hero
- why Temporis
- product split
- company / research section
- trust / responsible use
- final CTA
- footer

### Temporis Vista
File:
- `../vista.html`

Required sections:
- product hero
- who it is for
- what users see
- screenshot or chart gallery
- why visual forecasting workflow matters
- CTA for early access or product interest
- disclosure block

Visual rule:
- the page should work as an "imagining" page with bold type and meaningful motion or visual energy

Launch behavior:
- primary CTA should point to a local action for now, such as request access, join early access, or contact
- page should support a later CTA swap to `https://vista.temporis.co`
- page URL should remain `temporis.co/vista` until the dedicated product host is ready

### Temporis Platform
File:
- `../platform.html`

Required sections:
- product hero
- who it is for
- API overview
- example use cases
- request / response snippet
- access flow
- CTA for early access or API interest
- disclosure block

Visual rule:
- the page should work as an "imagining" page with bold type and meaningful motion or visual energy

Launch behavior:
- primary CTA should point to a local action for now, such as request API access, join early access, or contact
- page should support a later CTA swap to `https://platform.temporis.co`
- page URL should remain `temporis.co/platform` until the dedicated product host is ready

### Company
File:
- [about.html](../about.html)

Required sections:
- company summary
- mission
- market focus
- research / model explanation
- how the core engine powers Vista and Platform
- product-led structure
- team or company facts
- contact path

### Contact
File:
- [contact.html](../contact.html)

Required sections:
- contact intro
- inquiry type selector
- form
- direct email path
- response expectations

### Legal
Files:
- `../privacy.html`
- `../terms.html`
- `../disclaimer.html`

Required sections:
- clear heading
- last updated line
- readable legal body
- footer navigation

## 6. Component Mapping
Use a small static component vocabulary expressed through repeated HTML patterns and CSS classes.

### Global components
- `site-header`
- `site-nav`
- `site-logo`
- `button`
- `button-primary`
- `button-secondary`
- `section-shell`
- `section-intro`
- `site-footer`

### Marketing / product components
- `hero`
- `hero-copy`
- `hero-media`
- `product-split`
- `product-card`
- `media-frame`
- `trust-panel`
- `cta-band`
- `comparison-block`
- `imagining-hero`

### Technical components
- `code-block`
- `code-header`
- `metric-tag`
- `flow-diagram`

### Contact / legal components
- `contact-form`
- `select-group`
- `form-group`
- `legal-layout`
- `legal-meta`

## 7. CSS System Plan
Use one stylesheet for v1 unless it becomes unmanageable.

### CSS responsibilities in [styles.css](../styles.css)
- CSS custom properties for color, spacing, typography, radius, border, and motion
- base element styling
- layout utilities
- component classes
- page-specific section styling where necessary
- responsive breakpoints

### Responsive implementation rule
Every global component and every page section should be implemented with desktop and mobile behavior in mind from the start. Do not design desktop first and treat mobile as cleanup.

### Token groups to define
- colors
- font families
- type scale
- spacing scale
- border radius
- shadow levels
- container widths
- transition timing

### CSS rule
Do not implement page-specific visuals by piling ad hoc inline styles or one-off selectors into each page. Build reusable section and component classes first.

## 8. Content Implementation Rules

### Content status model
Every page section should be implemented with one of three statuses:

- final copy ready
- temporary structured placeholder
- asset pending

### Placeholder rule
If final copy or screenshots are not ready, use clearly structured placeholder content that preserves layout and hierarchy. Do not use lorem ipsum.

### Copy implementation rules
- use the full product names at first mention on each page
- keep paragraphs short
- keep headlines literal and clear
- avoid introducing new claims that are not in the PRD or design plan

### Interim-launch messaging rule
For `/vista` and `/platform`, avoid empty "coming soon" language. Instead, use product-intent language such as:

- preview
- early access
- request access
- product path
- currently launching from temporis.co

The pages should feel substantive enough to stand alone until the subdomains are live.

### Interim CTA pattern
For `/vista` and `/platform`, use one of these patterns consistently:

- primary CTA: request access
- secondary CTA: contact

or

- primary CTA: join early access
- secondary CTA: learn more

Do not mix one product page using "coming soon" while the other uses a stronger action model.

### Comprehension rule
Apply the same standards used in strong pitch decks:
- legible
- simple
- obvious

If a page section introduces a concept too early or forces the visitor to decode internal terminology, simplify it.

## 9. Asset Requirements

### Existing assets
- current logo files can be evaluated, but the implementation should not assume they are final

### Required assets for a strong v1
- one chosen logo lockup
- at least one Vista screenshot
- at least one Platform screenshot or interface capture
- one simple company or research system diagram if needed

### If assets are not ready
Use:
- framed placeholder panels labeled by asset role
- simplified inline SVG or CSS diagram blocks
- neutral mock interface compositions that communicate layout but avoid fake product claims

## 10. Navigation and Linking Rules

### Header
- present on every page
- same order on every page
- same top-level nav on all company-level pages

Top-level nav should remain:
- Products
- Company
- Contact

### Footer
- present on every page
- include legal links
- include product and company links

### Internal linking rules
- Home must link to Products, Company, and Contact
- Products must route clearly to Vista and Platform
- Company must link to Contact
- chart or forecast-heavy pages must link to Disclaimer
- during the interim phase, homepage product CTAs should link to `/vista` and `/platform`
- when the subdomains go live, those links can be switched to the subdomains without restructuring the page

## 11. Accessibility Checklist
Implementation is not complete unless all of the following are true:

- heading order is semantic
- nav is keyboard accessible
- focus state is visible on links, buttons, inputs, and menu items
- color contrast is sufficient for body text and controls
- forms use labels and clear error or hint structure
- images and diagrams have useful alt text
- mobile layout is readable without horizontal scrolling
- CTA buttons remain distinguishable without color alone

### Responsive checklist
Implementation is not complete unless:
- homepage works on both desktop and mobile
- header navigation remains understandable on mobile
- product pages keep their key CTA and disclosure visible on smaller screens
- forms remain usable on touch devices
- legal pages remain readable without cramped text columns
- the top navigation remains immediately understandable without prior product knowledge

## 12. SEO Checklist
Each page should include:

- unique title
- unique meta description
- canonical-friendly clean path assumptions
- semantic headings
- internal links to related pages

### Suggested title pattern
- `Temporis | AI Forecasting for Financial Markets`
- `Temporis Vista | Visual Forecasts`
- `Temporis Platform | Forecasting API Access`
- `Company | Temporis`
- `Contact | Temporis`

## 13. Analytics Plan
If analytics are added, track only essential events.

### Event list
- homepage vista CTA click
- homepage platform CTA click
- vista page CTA click
- platform page CTA click
- contact email CTA click
- top-nav product click

### Optional access events
- vista access CTA click
- platform access CTA click
- direct email click

### Rule
Do not block launch on analytics setup. Structure the markup so event hooks can be added cleanly later.

## 14. Phased Delivery Plan

### Phase 1: system and homepage
Deliver:
- rebuilt `styles.css`
- rebuilt `index.html`
- unified nav and footer
- initial brand expression

Acceptance:
- homepage clearly routes Vista vs Platform
- company story is clear in one screen and one scroll
- responsive layout works on mobile and desktop
- header remains understandable on mobile

### Phase 2: product pages
Deliver:
- `vista.html`
- `platform.html`

Acceptance:
- each page feels distinct but system-consistent
- product purpose is immediately clear
- access CTA targets are present
- disclosures appear where required
- each page can later change CTA destination to the subdomain without layout changes
- each page feels intentional and complete as a public product overview

### Phase 3: supporting pages
Deliver:
- rebuilt `about.html`
- rebuilt `contact.html`
- legal pages

Acceptance:
- company page feels factual and credible
- contact page is usable and low-friction
- legal pages are readable and linked sitewide

## 15. Recommended Work Order in This Repo

1. Rework [styles.css](../styles.css) into a tokenized design system.
2. Rebuild [index.html](../index.html) around the new homepage wireframe.
3. Create `vista.html` and `platform.html`.
4. Rewrite [about.html](../about.html) as the company page.
5. Rewrite [contact.html](../contact.html).
6. Create `privacy.html`, `terms.html`, and `disclaimer.html`.
7. Remove obsolete logo experiments and legacy pages that are no longer linked.
8. Run a final cross-page pass for nav consistency, copy consistency, accessibility, and SEO metadata.

## 16. Definition of Done
Implementation is complete when:

- all required pages exist
- navigation and footer are consistent across pages
- the site matches the information architecture in [design.md](design.md)
- the brand feels product-led, technically serious, and restrained
- all pages are responsive
- legal links exist and are reachable
- major CTAs route correctly
- placeholder content is clearly marked where final assets are pending
- `/vista` and `/platform` work as clear public product overview pages before subdomain launch
- the future redirect path to `vista.temporis.co` and `platform.temporis.co` is straightforward

Responsive quality specifically means the site is usable, legible, and structurally clear on both desktop and mobile.

Comprehension quality specifically means a first-time visitor can understand the company from the top navigation and first screen without decoding internal terminology first.

## 17. Immediate Next Step
The next practical step is to implement Phase 1:

- rebuild [styles.css](../styles.css)
- rebuild [index.html](../index.html)

That gives the project the visual system, navigation, and homepage structure needed for the rest of the site.
