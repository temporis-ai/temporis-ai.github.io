# Temporis Website Design Guide

## Purpose
This document defines the UX and design direction for the first public launch of the Temporis company website.

It should work with:

- [requirements.md](requirements.md) for launch scope and page requirements
- [company.md](company.md) for company content and message source

This document is about:

- user understanding
- page purpose
- visual hierarchy
- interaction patterns
- layout and tone

It is not the implementation plan. That belongs in [implementation.md](implementation.md).

## Design objective
The launch site should feel:

- clear
- serious
- useful
- low-hype
- technically credible

The site is not the product. It is the public front door to the company.

The design should help a first-time visitor understand:

- what Temporis is
- what each page is for
- that the company is real and technically serious

## External design principles used
This guide is informed by a few current design principles that consistently appear in mature public-facing web guidance:

- strong content hierarchy
- one dominant purpose per page section
- plain language before explanation
- scanning-friendly composition
- restraint over decoration

Useful references:

- GOV.UK content design guidance: users should understand quickly whether a page is relevant and not be forced through unnecessary explanation
- GOV.UK publishing design guidance: page structure should help users find what they need, not showcase internal complexity
- general visual hierarchy guidance: scale, spacing, and contrast should make the reading order obvious

Implication for Temporis:

- the site should not feel like a generic SaaS section stack
- layout variety is good when it reflects page purpose
- visual refinement should improve comprehension first

## Launch page set
Design for exactly these launch pages:

- `index.html`
- `product.html`
- `research.html`
- `company.html`
- `terms.html`

`terms.html` is footer-only.

## Core UX principle
Each page should do one thing well.

Do not design the site as one long mixed-purpose marketing surface.

The intended page roles are:

- Home: introduce Temporis at the company level
- Products: explain Vista and Platform
- Research: explain Collie
- Company: explain vision, nature, and contact
- Terms: provide legal text in a readable format

## Audience model
The launch site serves mixed audiences, but each page should still optimize for its own reading context.

### Home
Audience:

- general first-time visitors
- non-technical readers
- investors and partners
- curious technical readers

Design implication:

- plain language first
- low jargon
- interest before detail

### Products
Audience:

- people evaluating Vista
- developers evaluating Platform
- readers trying to understand what the company sells

Design implication:

- practical product framing
- clear product separation
- financial markets stated plainly

### Research
Audience:

- technically curious readers
- researchers
- investors looking for technical depth

Design implication:

- more technical language is acceptable
- technical terms must still be explained
- credibility comes from clarity, not density

### Company
Audience:

- people evaluating mission and seriousness
- investors, partners, and potential hires

Design implication:

- company language, not research jargon
- practical mission
- direct contact path

## Page-by-page UX direction

### Home
The homepage should introduce Temporis simply and create curiosity about what the company can do.

It should:

- stay at the company level
- lead with usefulness
- mention AI, but not in the first phrase
- avoid product detail
- avoid financial-market detail

Recommended reading flow:

1. Hero
2. What Temporis is
3. Why it matters / launch focus
4. Footer

Hero intent:

- clear
- interesting
- non-technical

The homepage should not:

- explain Collie in detail
- explain Vista and Platform in detail
- define finance as the homepage identity

### Products
The Products page should explain how Temporis turns forecasting into products people can use.

It should:

- introduce Vista first
- introduce Platform second
- mention financial markets as the first domain
- mention Collie lightly

Recommended reading flow:

1. Product page introduction
2. Vista
3. Platform
4. Short closing connection back to Temporis

Vista should feel:

- visual
- approachable
- practical

Platform should feel:

- technical
- controlled
- integration-ready

### Research
The Research page should make the research feel meaningful.

It should leave readers with the impression that:

- the model is real
- the company has real technical value
- the technology can grow stronger over time

Recommended reading flow:

1. Collie introduction
2. What a time series foundation model means
3. Multivariate
4. Multimodal
5. Why the capabilities matter
6. Finance as starting point, not limit

### Company
The Company page should feel practical and mission-led.

It should lead with:

- AI company identity
- better decisions under uncertainty
- forecasting technology made accessible through products and integrations

The Company page should feel:

- grounded
- serious
- useful

It should not feel like:

- a manifesto
- a research abstract
- a generic startup mission page

## Navigation UX
The header should use this order:

- `Temporis`
- `Products`
- `Research`
- `Company`
- `Try Vista`

Rules:

- brand anchors the left
- `Try Vista` is the only highlighted action
- informational links stay visually quieter
- desktop navigation should not wrap
- mobile navigation should simplify to menu, brand, and `Try Vista`

## Visual direction
The visual system should feel like:

- a calm AI company
- a serious forecasting company
- a restrained product website

Preferred cues:

- framed visuals
- chart-like structure
- light panels
- clear dividers
- strong typography hierarchy

Avoid:

- decorative futurism
- crypto/trading-signal styling
- heavy glow effects
- noisy dashboard mosaics
- generic consulting-site layouts

Refinement rules:

- use contrast in scale and spacing before adding more components
- prefer one strong panel over three weak ones
- let whitespace separate ideas instead of adding extra borders everywhere
- use page-specific emphasis so Home, Products, Research, and Company do not feel templated

## Tone and copy in design
Design and copy should work together.

The design should support copy that feels:

- direct
- useful
- understandable
- restrained

Design should not rely on visual drama to create meaning.

## Typography
Typography should carry much of the brand seriousness.

Guidelines:

- restrained headline sizing
- readable body size
- narrow copy measure
- strong difference between headline, body, labels, and legal text

Suggested families:

- `IBM Plex Sans`
- `Geist`
- `Instrument Sans`

Mono should be used only when it adds technical meaning.

## Color and surfaces
Use a restrained system:

- dark ink for primary text
- soft neutrals for surfaces
- one primary accent
- one support accent

The site should read as:

- premium
- technical
- calm

Not:

- flashy
- neon
- finance-hype

## Layout rules
Use a consistent system:

- narrow copy widths
- generous spacing
- left-aligned section starts
- simple responsive collapse

Rules:

- one dominant idea per section
- avoid more than one major focal point in a section
- avoid sections that combine too many unrelated messages
- use cards and panels sparingly and consistently
- vary section composition by page role, not by decoration
- keep long-form explanatory content in narrower measures than support content
- let supporting panels summarize or direct, not compete with the main copy

## Alignment invariants
These are not optional styling preferences. They are core layout rules for the launch site.

- The primary opening block on each page should follow one shared alignment logic.
- The first major section below the opening should not suddenly shift to a different horizontal anchor.
- Do not center a standalone panel above left-aligned body content unless the full page is intentionally centered.
- If a visual or card is removed from a layout, the layout must be recomposed so the remaining content still feels intentional.
- Similar page openings should share the same left edge, reading width, and vertical rhythm.

Practical meaning:

- Home, Products, Research, and Company should open on the same visual grammar unless there is a strong reason not to.
- A top section should not feel half-empty because it still assumes a removed right column.
- A centered card followed by left-anchored content usually reads as a mistake, not as structure.

Recommended structural patterns:

- Home: editorial intro, then orientation, then clear next paths
- Products: overview, domain framing, then product-by-product explanation
- Research: model-first explanation with ordered concept building
- Company: mission first, operating model second, contact last

## Responsive behavior
Responsive quality is part of the design, not cleanup after implementation.

Rules:

- mobile should preserve meaning, not just fit
- the header should stay understandable
- the homepage hero should remain readable in one column
- card layouts should stack cleanly
- desktop patterns should not be awkwardly compressed into mobile

## Accessibility by design
The design must support:

- semantic reading order
- strong contrast
- visible focus states
- readable text sizes
- non-color-only meaning

Accessible design is part of the brand impression.

## Design anti-patterns
Avoid:

- designing one page to do everything
- introducing jargon before context
- compensating hacks to fix layout problems
- navigation patterns that confuse first-time visitors
- visual systems that feel speculative or promotional rather than trustworthy

## Definition of design success
The design is successful when:

- each page has one clear purpose
- the site feels coherent across all launch pages
- the homepage is understandable to non-technical readers
- the Products page feels product-led
- the Research page feels technically serious
- the Company page feels mission-led and grounded
- the site looks calm, clear, and credible on desktop and mobile
