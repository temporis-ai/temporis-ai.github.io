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

- privacy page: `privacy.html`
- terms page: `terms.html`

`privacy.html` and `terms.html` should be linked in the footer only.
They should not appear as top-level navigation items.

These two pages are company-level legal surfaces.
They may be reused by products where appropriate, but they do not replace product-specific commercial terms such as Vista subscription terms.

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
- short company descriptor: `AI forecasting solutions`
- public contact email: `hello@temporis.co`
- link to `privacy.html`
- link to `terms.html`

The footer legal links are the shared company-level baseline.
Product-specific subscription terms should live with the product that owns the subscription.

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
- why the company matters

The homepage is an introduction, not a full explanation of everything.
It should stay simple and should not go into product or domain detail.
It should be understandable to a non-technical reader.

### Homepage primary goals
The homepage must do these things well:

1. Explain what Temporis is in plain language.
2. Explain why the company matters.
3. Establish technical credibility without hype.
4. Show that research and product belong to one company.

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
3. Why it matters
4. Footer

#### Hero
The hero must include:

- the company name
- a plain-language headline
- a short supporting explanation

The hero headline should answer:

- what the company builds

The hero should avoid unexplained technical terms such as:

- time series
- multimodal
- multivariate
- TSFM

#### What Temporis Is
This section should explain the company at a slightly broader level.

It should explain that Temporis is an AI company focused on forecasting and that research and product belong to the same company.

#### Why It Matters
This section should explain why better forecasting matters in simple terms.

It may use supporting cards or panels, but they should read as one coherent row rather than navigation aids.

#### Footer
The homepage footer must include:

- company name
- short company descriptor
- public contact email: `hello@temporis.co`
- legal link to `privacy.html`
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

Vista and Platform should use the same layout pattern:

- text on the left
- visual panel on the right

The Products page may use more concrete domain language such as:

- market data
- forecasts
- charts
- API

But it should still avoid unexplained research jargon.

## Research page requirements
The Research page applies to `research.html`.

### Research page objective
The Research page should introduce Collie as the Temporis time series forecasting foundation model.
This page can be more technical than the rest of the site.
It should make the research feel meaningful and show long-term company value and potential.

### Research page required content
The Research page must include:

- a single merged opening section introducing Collie
- Collie as the core forecasting model at Temporis
- time series forecasting foundation model as the model category
- multivariate capability
- multimodality
- a clear statement that the research is built to advance the state of the art in forecasting

The Research page should stay focused on the model and not expand into product-market detail.
Unlike the homepage, this page may use technical terms directly, but they should still be explained well enough for an interested non-specialist reader.
Technical explanation should follow a clear order inside the opening section:

1. time series
2. multivariate
3. multimodality

If the page mentions finance, it should present finance as the starting point for Collie, not the limit of where it can be useful.

The page should imply long-term product and company value through the model's broader usefulness and ability to grow stronger over time, without turning into a product page.

## Company page requirements
The Company page applies to `company.html`.

### Company page objective
The Company page should explain what kind of company Temporis is, what its mission is, and how to contact it.

### Company page required content
The Company page must include:

- a Company section that states Temporis is an AI company that develops forecasting technology
- a statement that research and product are connected from the start
- a Mission section about delivering advanced forecasting technology to people
- a statement that Temporis makes forecasting technology accessible through products and integrations
- product and integration delivery paths
- public contact information

The Company page should inspire confidence without becoming a manifesto.
This page should speak in company language rather than research language.
`Company`, `Mission`, and `Contact` should read as separate sections, but should still use one consistent page system rather than switching into a different callout style for contact.

The Company page should help a general reader understand:

- what kind of company Temporis is
- what its mission is
- how to contact it

The page should lead with:

- Temporis as an AI company
- forecasting technology as the company focus

It should then explain that Temporis delivers this through products and integrations.

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

## Shared legal-surface requirements

### Privacy page role
`privacy.html` should act as the shared company-level privacy policy for Temporis website surfaces and public product surfaces that choose to link to it.

It should be allowed to mention shared product-supporting concepts such as:

- authentication
- billing-state handling
- service providers
- privacy contact paths

These references should stay company-level and operational.
They should not turn the page into product-specific subscription or account-management documentation.

### Terms page role
`terms.html` should act as a company-level terms-of-use page for the Temporis website and other company-owned public informational surfaces that link to it.

It should:

- stay focused on company-level website and informational-use terms
- preserve the low-hype and no-guarantee posture
- avoid pretending to be the commercial subscription agreement for Vista

### Product-specific commercial terms
If a product needs subscription, billing, refund, renewal, cancellation, or account-rule terms that go beyond the company-level baseline, those terms should live in the product repo that owns that product.

For launch planning:

- company-level privacy and baseline terms live in this repo
- Vista-specific subscription terms live in the Vista repo

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

- `index.html`, `product.html`, `research.html`, `company.html`, `privacy.html`, and `terms.html` all exist
- the main navigation clearly communicates the site structure
- `privacy.html` and `terms.html` are linked from the footer and not treated as top-level pages
- a first-time visitor can understand what Temporis is within one screen and one scroll of the homepage
- the site feels serious, focused, and low-hype
- the pages work cleanly on desktop and mobile
- the copy can be traced back to [company.md](company.md)
