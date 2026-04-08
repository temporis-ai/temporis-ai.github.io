# Temporis Website Implementation Plan

## Purpose
This document defines how to implement the launch website described in:

- [requirements.md](requirements.md)
- [company.md](company.md)
- [design.md](design.md)

It covers:

- file structure
- implementation order
- page mapping
- component mapping
- content rules
- responsive behavior
- completion criteria

## Implementation model
The launch site is a static website.

The goal is to implement a clean, maintainable v1 using:

- HTML
- CSS
- existing static assets where needed

Do not implement extra infrastructure unless it is required for launch.

## Launch files
The implementation should support these files:

- [index.html](../index.html)
- [product.html](../product.html)
- [research.html](../research.html)
- [company.html](../company.html)
- [terms.html](../terms.html)
- [styles.css](../styles.css)

Legacy files such as `about.html`, `contact.html`, `vista.html`, `platform.html`, `privacy.html`, and `disclaimer.html` should not drive the current implementation plan.

## Build order
Implement the site in layers.

### Layer 1: shared system
- global CSS tokens
- layout containers
- typography
- header
- footer
- buttons and links
- card and panel patterns

### Layer 2: homepage
- hero
- supporting company sections
- footer integration

### Layer 3: inner pages
- Products page
- Research page
- Company page
- Terms page

### Layer 4: consistency pass
- responsive review
- accessibility review
- copy consistency
- navigation and footer consistency

## Page-to-file mapping

### Home
File:

- [index.html](../index.html)

Purpose:

- company-level introduction

Required sections:

- shared header
- hero
- what Temporis is
- why it matters / launch focus
- shared footer

### Products
File:

- [product.html](../product.html)

Purpose:

- explain Vista and Platform

Required sections:

- shared header
- page introduction
- Vista section
- Platform section
- short closing connection to Temporis
- shared footer

### Research
File:

- [research.html](../research.html)

Purpose:

- explain Collie

Required sections:

- shared header
- Collie introduction
- explanation of time series
- explanation of multivariate
- explanation of multimodal
- why the capabilities matter
- finance as starting point
- shared footer

### Company
File:

- [company.html](../company.html)

Purpose:

- explain mission, nature, and contact

Required sections:

- shared header
- company introduction
- mission / better decisions under uncertainty
- forecasting technology through products and integrations
- contact section
- shared footer

### Terms
File:

- [terms.html](../terms.html)

Purpose:

- readable legal page

Required sections:

- shared header
- title
- last updated line
- legal body
- shared footer

## Shared component mapping
Use a small repeated component vocabulary.

### Global components
- `site-header`
- `site-nav`
- `site-logo`
- `nav-try`
- `section-shell`
- `section-intro`
- `site-footer`

### Content components
- `hero`
- `hero-copy`
- `feature-card`
- `surface-panel`
- `note-panel`
- `bridge-panel`
- `sequence-item`
- `legal-shell`

### Optional visual components
- `media-frame`
- `chart-mock`
- `mini-chart`
- `mini-code`
- `metric-tag`

Only keep optional components if they support the current launch pages.

## CSS system rules
Use one shared stylesheet for launch.

`styles.css` should own:

- color tokens
- typography tokens
- spacing scale
- container widths
- shared layout classes
- reusable page-section patterns
- responsive breakpoints

Rules:

- do not solve page-specific layout needs with ad hoc one-off selectors first
- prefer reusable classes over deeply page-specific rules
- keep the system small enough to understand

## Content implementation rules
Page copy should come from [company.md](company.md).

Rules:

- do not invent new company claims during implementation
- keep headlines literal and clear
- keep paragraphs short
- keep page language appropriate to page audience

Audience reminders:

- Home: plain language
- Products: practical product language
- Research: technical but explained
- Company: mission and company language

## Navigation rules
Every launch page should use the same top navigation:

- `Products`
- `Research`
- `Company`
- `Try Vista`

The brand should link to `index.html`.

`terms.html` should appear only in the footer.

## Footer rules
Every launch page should use a shared footer that includes:

- company name
- short descriptor
- `hello@temporis.co`
- `terms.html`

## Responsive implementation rules
Responsive behavior must be built in from the start.

Rules:

- do not build desktop first and patch mobile later
- test the header early
- stack page sections cleanly at smaller widths
- keep readable spacing and type sizes on mobile
- preserve section order when collapsing layouts

## Accessibility rules
Implementation is not complete unless:

- heading order is semantic
- keyboard focus is visible
- contrast is strong enough for text and controls
- alt text is used where needed
- navigation works by keyboard
- pages remain usable without horizontal scrolling

## SEO rules
Each launch page should have:

- unique title
- unique meta description
- semantic headings
- crawlable internal links

## Placeholder rule
If a visual asset is not ready:

- use a structured placeholder
- keep the intended layout
- do not use lorem ipsum
- do not imply product claims that are not real

## Work order in this repo

1. Align [styles.css](../styles.css) with the shared launch system.
2. Rework [index.html](../index.html) to match the homepage requirements.
3. Rework [product.html](../product.html).
4. Rework [research.html](../research.html).
5. Rework [company.html](../company.html).
6. Rework [terms.html](../terms.html).
7. Run a full cross-page consistency pass.

## Definition of implementation done
Implementation is done when:

- the five launch files exist and are coherent
- navigation and footer are consistent across pages
- the pages follow [requirements.md](requirements.md)
- the pages draw from [company.md](company.md)
- the UX matches [design.md](design.md)
- the site works on desktop and mobile
- the site remains clear and low-hype

## Immediate next step
The next practical step is:

1. align [index.html](../index.html) to the current docs
2. adjust [styles.css](../styles.css) only as needed to support that page cleanly
