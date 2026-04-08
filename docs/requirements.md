# Temporis Launch Website Requirements

## Purpose
This document is the single source of truth for the requirements of the first public launch of the Temporis company website.

It defines:

- what pages must exist for launch
- what each page is for
- what the homepage must communicate
- what the launch site must avoid

This document defines requirements and scope.
It does not define the company content source. That belongs in [company.md](company.md).

## Document model
Use the two-document system below:

- `requirements.md` defines launch scope, page requirements, and constraints.
- `company.md` defines company facts, positioning, safe claims, and source content.

If there is a conflict:

- `requirements.md` decides structure and scope
- `company.md` decides substance and wording direction

## Launch scope
The first public launch should be a simple company website, not a large marketing site and not the product itself.

The launch website must include these pages:

- main homepage: `index.html`
- products page: `product.html`
- research page: `research.html`
- company page: `company.html`

The launch website must also include:

- terms page: `terms.html`

`terms.html` should be linked in the footer only.
It should not appear as a top-level navigation item.

## Launch navigation
The top-level public navigation for launch should be:

- `Products`
- `Research`
- `Company`
- `Try Vista`

The brand `Temporis` should anchor the header and link to the homepage.

## Launch objective
The launch site should work as the public front door to the company.

On a first visit, a reader should quickly understand:

- Temporis is the company
- Temporis helps people uncover patterns and make better decisions
- the company is research-driven and product-led

The launch site should feel clear, serious, and intentionally narrow in scope.

## Site-wide requirements

### Required structure
The site structure must be immediately legible:

- `index.html` explains the company at a high level
- `product.html` explains Vista and Platform
- `research.html` explains Collie
- `company.html` explains vision, nature, and contact

### Required footer behavior
All launch pages should include a footer with:

- company name
- short company descriptor
- public contact email: `hello@temporis.co`
- link to `terms.html`

### Required quality bar
The launch site must be:

- clear
- credible
- low-hype
- easy to navigate
- responsive on desktop and mobile

### Non-goals
The launch site should not:

- try to explain everything on one page
- make hard-to-support performance claims
- present the company like a consultancy
- behave like a generic SaaS template
- feel like a crypto or trading-signals site

## Homepage requirements
The homepage is the most important page in the launch set.

It applies to:

- URL: `https://temporis.co/`
- file: `index.html`

### Homepage objective
The homepage should work as the front door to the company.

On a first visit, a reader should quickly understand:

- what Temporis is
- what the company builds
- how Product, Research, and Company fit together

The homepage is an introduction, not a full explanation of everything.
It should stay simple and should not go into product or domain detail.
It should be understandable to a non-technical reader.

### Homepage primary goals
The homepage must do these things well:

1. Explain what Temporis is in plain language.
2. Make the company structure legible.
3. Establish technical credibility without hype.
4. Show that research and product belong to one company.
5. Make it easy to continue into the rest of the site.

### Homepage audience
The homepage should work for a mixed first-visit audience:

- prospective users
- technical evaluators
- investors and partners
- press and ecosystem visitors

The page should not assume prior familiarity with:

- time series modeling
- forecasting terminology
- product names
- internal research names such as Collie

### Homepage core message
At minimum, the homepage must communicate this:

Temporis helps people uncover patterns in things like prices and demand, and make better decisions.

It should also make these supporting ideas clear:

- research is the technical engine
- product is how the capability reaches users
- the company exists to make advanced forecasting more accessible and useful

### Homepage required sections
The homepage should remain short and narrowly scoped.

Required reading flow:

1. Hero
2. What Temporis is
3. Launch focus
4. Footer

#### Hero
The hero must include:

- the company name
- a plain-language headline
- a short supporting explanation
- a visible trust or restraint line

The hero headline should answer:

- what the company builds

The hero should avoid unexplained technical terms such as:

- time series
- multimodal
- multivariate
- TSFM

#### What Temporis Is
This section should explain the company at a slightly broader level.

It must clarify that Temporis has three public company surfaces:

- Product
- Research
- Company

These should be explained as parts of one company, not as disconnected offerings.

This section may introduce the idea of forecasting, but should still use plain language first.

#### Launch Focus
This section should explain the launch posture.

It must cover:

- why Temporis matters in simple terms
- why the launch site is intentionally simple

#### Footer
The homepage footer must include:

- company name
- short company descriptor
- public contact email: `hello@temporis.co`
- legal link to `terms.html`

### Homepage content requirements
Homepage copy must be:

- concise
- technically grounded
- low-hype
- understandable on a first read

Copy should avoid:

- consulting language
- generic AI buzzwords
- inflated market claims
- performance promises
- investment-advice language
- unexplained internal terms

The homepage should avoid domain-specific detail.
Financial markets should not be a homepage focus.
If technical language is used on the homepage, it should be explained immediately in plain language.

### Homepage required meanings
The homepage should make these distinctions legible:

- Temporis is the company
- Vista is a product surface, not the company
- Collie is a research effort, not the public top-level brand
- research and product are connected, not separate narratives

## Product page requirements
The Products page applies to `product.html`.

### Product page objective
The Products page should introduce the two product surfaces:

- Vista
- Platform

It should explain how Temporis turns forecasting into products people can use.
It should explain what each product is for and how they differ.

This is the page where the financial-markets domain should be stated clearly.
This page can be more specific than the homepage because readers are now looking for product detail.

### Product page required content
The Products page must include:

- Vista as a forecast gallery
- Platform as an API product
- a light mention of Collie
- financial markets as the initial domain

The Products page should explain product value in user terms:

- Vista helps people read forecasts through charts
- Platform helps developers access forecasting through an API
- the products are built for financial-market use cases first

### Product page required meanings
The Products page should make these distinctions clear:

- Vista provides charts
- Platform provides API access
- the underlying model is Collie
- the product focus is financial markets

The page should explain the two products in a simple user sequence:

- Vista helps users read forecasts, explore them, and use them in strategy
- Platform helps developers access Collie, control model behavior, and integrate it into their own systems

The Products page may use more concrete domain language such as:

- market data
- forecasts
- charts
- API

But it should still avoid unexplained research jargon.

## Research page requirements
The Research page applies to `research.html`.

### Research page objective
The Research page should introduce Collie as the Temporis time series foundation model.
This page can be more technical than the rest of the site.
It should make the research feel meaningful and show long-term company value and potential.

### Research page required content
The Research page must include:

- Collie as the core forecasting model at Temporis
- TSFM as the model category
- multivariate capability
- multimodality
- a clear statement that the research is built to advance the state of the art in forecasting

The Research page should stay focused on the model and not expand into product-market detail.
Unlike the homepage, this page may use technical terms directly, but they should still be explained well enough for an interested non-specialist reader.
Technical explanation should follow a clear order:

1. time series
2. multivariate
3. multimodality

If the page mentions finance, it should present finance as the starting point for Collie, not the limit of where it can be useful.

The page should imply long-term product and company value through the model's broader usefulness and ability to grow stronger over time, without turning into a product page.

## Company page requirements
The Company page applies to `company.html`.

### Company page objective
The Company page should explain the vision and nature of the company.

### Company page required content
The Company page must include:

- company vision
- company nature
- a statement that Temporis is an AI company helping people and businesses make better decisions under uncertainty
- a statement that Temporis develops forecasting technology and makes it accessible through products and integrations
- public contact information

The Company page should inspire confidence without becoming a manifesto.
This page should speak in company language rather than research language.

The Company page should help a general reader understand:

- why the company exists
- what kind of company it wants to be
- how to contact it

The page should lead with:

- Temporis as an AI company
- helping people and businesses make better decisions under uncertainty

It should then explain that the company develops forecasting technology and makes it accessible through products and integrations.

## Launch claims and trust requirements
The launch site must establish trust through restraint.

Requirements:

- no guaranteed-outcome language
- no unsupported model-performance claims
- no investment-advice framing
- no exaggerated product claims

The site may talk about:

- decision support
- forecasting intelligence
- research direction
- product direction

The site should avoid:

- public benchmark claims unless separately reviewed
- trading-performance language
- language that implies certainty

## Responsive requirements
Responsive quality is required for launch.

The launch pages must:

- work clearly on desktop and mobile
- preserve hierarchy when stacked
- keep navigation understandable on smaller screens
- avoid awkward multi-row header behavior
- keep tap targets usable on touch devices

## Accessibility requirements
The launch pages must:

- use semantic heading order
- keep visible keyboard focus styles
- maintain readable text contrast
- avoid conveying meaning by color alone
- remain usable with keyboard navigation

## SEO and metadata requirements
Each launch page must have:

- a unique title
- a unique meta description
- clear language aligned with actual visitor intent
- crawlable navigation links

## Definition of done
The launch website requirements are satisfied when:

- `index.html`, `product.html`, `research.html`, `company.html`, and `terms.html` all exist
- the main navigation clearly communicates the site structure
- `terms.html` is linked from the footer and not treated as a top-level page
- a first-time visitor can understand what Temporis is within one screen and one scroll of the homepage
- the site feels serious, focused, and low-hype
- the pages work cleanly on desktop and mobile
- the copy can be traced back to [company.md](company.md)
