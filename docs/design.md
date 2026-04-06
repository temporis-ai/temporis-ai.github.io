# Temporis Website Design Plan

## 1. Objective
Design the public company website for Temporis so a first-time visitor can immediately understand:

- Temporis is the company.
- Vista is the visual forecast product.
- Platform is the API product.
- The company is credible, technically serious, and product-led.

This site is the public narrative layer, not the product itself.

It must work clearly and reliably on both desktop and mobile.

## 2. Immediate Design Conclusion
The current site direction is too generic and consulting-like for the PRD. It uses broad strategy language, a standard corporate layout, and a navigation model built around `Services` / `About Us`, which conflicts with the required product-led company story.

The new design should reposition Temporis as:

- an AI company, not an analytics consultancy
- a forecasting company, not a general data advisory business
- a product company with two clear user paths
- a serious, restrained brand with trust signals built into the interface

## 3. Brand Strategy

### Core brand idea
Temporis should feel like a calm forecasting infrastructure company with visible products.

### Positioning sentence
Temporis is a forecasting AI company that turns foundation-model capabilities into usable products for market-facing decision support.

### Brand attributes
- Precise
- Quiet
- Technical
- Trustworthy
- Rigorous
- Modern

### Emotional target
The site should make visitors think:

- This company is focused.
- The products are real.
- The model layer is serious.
- The company explains complex things clearly.

### Brand anti-patterns
Avoid:

- consulting-firm language
- hype-heavy AI language
- trading-signal aesthetics
- crypto-style neon dashboards
- decorative futurism with no explanatory value

### Brand promise
The website should promise only what the company can visibly support:

- clear product structure
- serious forecasting technology
- usable interfaces
- careful communication

### Brand tension to balance
The brand has to hold two ideas at once:

- advanced model company
- practical product company

If the site leans too far toward research, it will feel abstract. If it leans too far toward marketing, it will lose technical credibility. The design should keep the model story visible inside the company narrative while Vista and Platform remain the entry points for most visitors.

### Naming rule
Use the product names consistently across navigation, headings, metadata, and CTAs:

- `Temporis` for the company
- `Temporis Vista` for the visual product
- `Temporis Platform` for the API product

Shortened labels like `Vista` and `Platform` are acceptable only in repeated UI contexts after the full names have already been established on the page.

`Collie` can still appear in company copy, but it should not be required as a top-level navigation concept.

## 4. Research-Based Design Principles
The design system should be built around current web best practices and patterns used by strong product-led technology brands.

### 4.0 Pitch-Deck Clarity Rule
The site should borrow the strongest communication rules from good pitch decks:

- make it legible
- make it simple
- make it obvious

From YC's guidance on pitch decks, the main idea is that people remember only a few ideas after a short presentation, and understanding has to come before memory. For the website, that means fewer top-level concepts, fewer competing messages, and one obvious idea per section.

### 4.1 Clarity before density
Nielsen Norman Group's visual design guidance emphasizes scale, hierarchy, contrast, and grouping to guide attention. For Temporis, that means one dominant message per section, limited emphasis styles, and a clear order of reading rather than stacked marketing claims.

### 4.2 Short text measures and readable rhythm
Baymard's readability guidance recommends body text around 50 to 75 characters per line, with readable spacing. This matches the PRD: narrow text columns, short paragraphs, and generous vertical rhythm will make the company appear more mature and easier to trust.

### 4.3 Accessibility is part of brand quality
`web.dev` accessibility guidance reinforces that color cannot carry meaning alone, contrast must be strong, and focus states must remain visible. For Temporis, accessible interaction should not be treated as a compliance afterthought. It directly supports the company's "careful and serious" positioning.

### 4.4 Responsive simplicity
`web.dev` responsive design guidance supports simple fluid layouts over device-specific page designs. The site should collapse from a two-column desktop rhythm to a single-column mobile flow without changing the information hierarchy.

Responsive behavior is not secondary polish. It is part of the core brand impression and comprehension model.

### 4.5 Trust is visual, not only verbal
For a company operating in financial-market forecasting, trust comes from restrained claims, stable typography, real product imagery, clean disclosures, and consistent design. The interface itself should signal discipline.

## 5. Reference Site Observations
These are not templates to copy. They are reference points for patterns that are working now.

### OpenAI Business
Useful pattern:
- very clear split between two buyer paths
- product screenshots carry the message
- trust content is integrated, not buried

Takeaway for Temporis:
- split Vista and Platform early on the homepage
- show each product in its native form
- explain the model-product relationship in plain language

### Anthropic
Useful pattern:
- restrained tone
- research and trust positioned as part of the company identity
- minimal hype in the visual language

Takeaway for Temporis:
- keep the homepage intellectually calm
- make responsible-use language visible
- let structure and typography do more work than visual effects

### Stripe
Useful pattern:
- strong product architecture
- clear section sequencing
- evidence and operational credibility integrated throughout

Takeaway for Temporis:
- use modular sections with clear handoff points
- reinforce company seriousness with proof, explanations, and product depth
- keep CTAs clear and repeated, not aggressive

## 6. Recommended Visual Direction

### Direction name
Structured Signal

### Summary
The visual language should feel like forecast infrastructure presented with editorial discipline.

### One-sentence art direction
Think "financial research terminal meets premium product site," but quieter, more open, and more legible.

### Visual cues
- fine grid structures
- soft panel boundaries
- restrained use of charts and forecast lines
- layered horizontal bands suggesting time windows
- sparse data marks and probability cues
- subtle diagrammatic framing around product visuals

### Composition rules
- Every major section should have one dominant focal point.
- Screenshots should be framed, cropped, and annotated rather than dumped raw.
- Use empty space as part of the composition, not as leftover area.
- Use lines, dividers, and light surface changes to create structure instead of heavy decoration.
- Limit any one section to one visual idea: screenshot, diagram, comparison, or trust statement.

### Avoid
- glowing blobs
- generic AI particles
- oversized gradients with no semantic role
- busy dashboard mosaics
- full-bleed hero art that obscures the message

## 7. Color System
Use mostly neutrals, with one strong brand accent and one restrained support accent.

### Recommended palette
- `Ink` `#0F1722`
- `Slate` `#4A5565`
- `Mist` `#E9EEF2`
- `Cloud` `#F7F9FB`
- `White` `#FFFFFF`
- `Horizon Blue` `#2563EB`
- `Signal Teal` `#0F8C82`

### Usage rules
- `Ink`, `Slate`, `Cloud`, and `White` should carry most of the interface.
- `Horizon Blue` should be the primary action color for links, CTAs, and active states.
- `Signal Teal` should be used sparingly for diagrams, tags, or non-primary highlights.
- Chart colors should be separate from the brand accent set so charts remain legible and semantically meaningful.

### Surface model
- Background: `Cloud` or `White`
- Primary text: `Ink`
- Secondary text: `Slate`
- Hairlines and panel borders: `Mist`
- Action emphasis: `Horizon Blue`
- Technical or analytical highlight: `Signal Teal`

### Contrast rule
The palette should be tested so body text, buttons, form controls, and link states all meet accessible contrast targets before visual polish work begins.

### Why this direction
This keeps the site technical and premium without looking cold, playful, or speculative.

## 8. Typography
Typography should be the main brand differentiator after the wordmark.

### Recommendation
Use one high-quality sans family across the site, with a mono companion only for code and data labels.

### Suggested options
- Primary: `Geist`, `IBM Plex Sans`, or `Instrument Sans`
- Mono: `IBM Plex Mono` or `Geist Mono`

### Type rules
- Headlines should be controlled, not oversized.
- Body text should sit in a narrow measure.
- Metadata, labels, and disclaimers should have a distinct smaller scale.
- Use mono only where it adds product or technical meaning.

### Suggested scale
- Hero headline: `48-64px`
- Section headline: `28-36px`
- Body: `16-18px`
- Small metadata / labels: `12-14px`
- Code / API snippets: `13-15px`

### Weight guidance
- Headlines: medium to semibold
- Body: regular
- UI labels: medium
- Avoid heavy bold usage except for very short emphasis

### Tone target
The typography should feel engineered, not fashionable.

## 9. Layout System

### Grid
- 12-column desktop grid
- 6 to 8-column tablet adaptation
- single-column mobile stack with preserved content order

### Content widths
- body copy max width: `60ch` to `70ch`
- dense explanatory sections max width: `60ch`
- product media areas can extend wider than text

### Section rhythm
- use large vertical spacing between sections
- keep section headers short
- avoid placing too many competing messages above the fold

### Containers
Use consistent outer gutters and restrained card radii. Panels should feel precise, not soft and consumer-app-like.

### Alignment rule
Favor hard left alignment and consistent section starts. Centered text should be used only in the hero and short CTA bands.

### Density rule
If a section needs more than three major visual objects, it likely needs to be split in two.

## 10. Information Architecture

### Domain model
- `temporis.co` or `www.temporis.co` is the company website.
- `temporis.co/vista` is the public product overview page for Temporis Vista.
- `temporis.co/platform` is the public product overview page for Temporis Platform.
- future destination domains:
  - `vista.temporis.co`
  - `platform.temporis.co`

### Launch-stage rule
For the first public version, the company site should present Vista and Platform as clear product overview pages inside the main domain. Access should route through the contact path until the dedicated product hosts are ready.

### Primary nav
- Products
- Company
- Contact

### Navigation behavior
- Header should remain compact and sticky.
- The active page should be visually clear without relying only on color.
- The top-level navigation should explain the site structure immediately.
- `Products` should be a clear umbrella label without extra explanatory text in the header.
- Product choices should happen inside the Products page, not in the top-level navigation.
- On mobile, the nav should stay short and immediately understandable.

### CTA hierarchy
- Product routing should happen inside the Products page and supporting CTA blocks, not through competing header buttons.
- Contact should remain a supporting path, not the dominant conversion pattern on every page.

### Footer
- Vista
- Platform
- Company
- Contact
- Privacy
- Terms
- Disclaimer

## 11. Homepage Strategy
The homepage should explain the company, branch the audience, and establish trust.

### Homepage design objective
Within the first screen and one scroll, a visitor should understand:

- what Temporis does
- the difference between Vista and Platform
- which path is for them
- that the company is serious and credible

### 11.1 Hero
Structure:
- concise company statement
- one supporting sentence
- one clear route into Products
- one meaningful visual

Recommended message shape:
- Headline: Temporis builds AI forecasting products for financial markets.
- Support: Temporis turns forecasting technology into products for visual users and technical builders.

Hero visual options:
- cropped Vista forecast chart in a clean frame
- a simple research to product relationship diagram
- a combined screenshot-plus-diagram composition

Recommended layout:
- Left: headline, support copy, primary CTA, one short trust line
- Right: framed product visual with minimal annotation

Trust line example:
- Built for decision support in time-series forecasting. No guaranteed outcomes.

### 11.2 Why Temporis
A short three-part explanation:
- why forecasting matters
- why forecasting technology improves the workflow
- why the company is starting with short-term financial markets

Recommended presentation:
- three compact columns on desktop
- stacked explanation cards on mobile
- each point limited to one heading and two short sentences

### 11.3 Product split
This is the most important homepage section after the hero.

Use two side-by-side product panels:

- Vista
  - For users who want visual forecasts
  - Show chart-led interface
  - CTA: View Vista

- Platform
  - For builders who want model access
  - Show API or schema-led interface
  - CTA: Get API access

Design requirements:
- make the two cards visually equal in weight
- differentiate them by content and visual style, not by louder color
- Vista should feel visual-first
- Platform should feel system-first
- link to `/vista` and `/platform` for the initial launch phase
- allow the CTA destinations to be swapped later to `vista.temporis.co` and `platform.temporis.co` without redesigning the sections

### 11.4 Company / research section
Fold the model story into the company story rather than isolating it as a separate concept.

Content frame:
- why the company exists
- what research or model work underpins the products
- how the core forecasting engine powers Vista and Platform
- why the company is starting with short-term financial markets

The goal is credibility without adding a top-level concept visitors have to decode.

### 11.5 Trust and responsible use
This should be a real section, not a disclaimer footnote.

Include:
- financial-market forecasting context
- decision-support framing
- no guaranteed outcomes
- careful claims language

Recommended treatment:
- muted panel background
- short factual statements
- optional link to full disclaimer
- no alarmist legal styling

### 11.6 Final CTA
Route people clearly into Products or Contact, depending on intent.

### 11.7 Recommended homepage wireframe
1. Header
2. Hero with one primary CTA into Products
3. Why Temporis
4. Vista / Platform split
5. Company / research section
6. Trust and responsible use
7. Final CTA
8. Footer

## 12. Page Plans

### Vista page
Tone:
- visual
- focused
- practical

Content blocks:
- who it is for
- what users see
- forecast chart examples
- workflow value
- access or early access CTA
- risk disclosure

Design note:
This page can use more chart imagery than the rest of the site, but the surrounding layout should stay calm.

Launch-state note:
This page should communicate a real product direction now, even if the full hosted Vista experience is not yet live. It should feel like an intentional "imagining" page: bold, visual, and future-facing, not a vague teaser.

Preferred section order:
1. Product hero
2. What users see
3. Why the visual workflow matters
4. Screenshot gallery or chart sequence
5. Access / early access CTA
6. Disclosure

### Platform page
Tone:
- technical
- clear
- integration-ready

Content blocks:
- who it is for
- what the API provides
- example inputs and outputs
- code snippet
- access flow
- access or early access CTA

Design note:
Use structured code blocks and system diagrams, not dense docs-style prose.

Launch-state note:
This page should present Temporis Platform as an upcoming but concrete builder product. It should also feel like an intentional "imagining" page: clear, bold, and future-facing before the dedicated subdomain is available.

Preferred section order:
1. Product hero
2. API overview
3. Use cases
4. Request / response example
5. Access / early access flow
6. CTA

### Company page
Tone:
- factual
- concise
- confident

Content blocks:
- mission
- why time-series forecasting
- current market wedge
- core research / model story
- how the engine powers Vista and Platform
- team section if ready
- contact path

Preferred section order:
1. Company summary
2. Mission
3. Why this market and wedge
4. Research / model explanation
5. Product-led company structure
6. Team or company facts
7. Contact path

Design note:
This page should read like a serious company brief, not an about-us lifestyle page.

### Contact page
Content blocks:
- short intro
- inquiry type selector
- email and form
- expectations for response

Suggested inquiry types:
- Product
- API / enterprise
- Partnership
- Investor / press
- General

Preferred section order:
1. Contact intro
2. Inquiry type selection
3. Form
4. Direct email path
5. Response expectations

Design note:
The form should feel practical and low-friction. Avoid large marketing copy blocks on this page.

### Legal pages
These should be plain, readable, and visually consistent with the rest of the site. They should feel maintained, not outsourced.

Required pages:
- Privacy
- Terms
- Disclaimer / Risk disclosure

Design note:
Use the same typography system and spacing discipline as the main site, but remove promotional distractions.

## 13. Core Component System
The initial component set should stay small and disciplined.

### Components
- header with compact nav and CTA pair
- primary and secondary buttons
- section intro block
- dual product cards
- screenshot frame
- code snippet block
- trust / disclosure block
- FAQ or limitations accordion if needed
- contact form
- footer

### Missing-but-required design patterns
- legal page template
- inquiry type selector
- inline disclaimer treatment near charts or performance-adjacent content
- product CTA band
- simple comparison or split-layout block for Vista vs Platform
- "imagining" hero treatment for interim product pages

### Component design characteristics
- corners should be restrained, not playful
- borders should be light but visible
- shadows should be soft and sparse
- hover states should rely on border, tint, or slight lift, not dramatic animation
- code blocks should feel product-grade, not developer-blog casual

### Component behavior rule
Each component must support one of three jobs:
- explain
- route
- reassure

If a component does none of those, it should not exist in v1.

## 14. Imagery and Motion

### Imagery
Priority order:
- real Vista screenshots
- real Platform captures
- simplified diagrams
- chart crops

Avoid stock photography unless there is a strong reason.

### Screenshot rules
- hide unnecessary UI clutter
- crop to one meaningful workflow
- annotate only the most important signal
- use consistent frame treatment across the site

### Diagram rules
- use horizontal flows where possible
- label in plain language
- keep node counts low
- do not mimic academic paper figures

### Motion
Keep it light:
- fade-and-rise section reveals
- subtle hover elevation or border shift
- simple chart transition or masked reveal
- clear nav and focus feedback

No cinematic hero animation.

## 15. Logo Direction

### Recommendation
Use a two-part identity for v1:

- a custom `Temporis` wordmark
- a distinct `TS` logo mark

### Wordmark qualities
- stable
- readable at small sizes
- works in one color
- credible in both product and investor contexts

### `TS` mark qualities
- simple enough for favicon and app-icon use
- memorable in silhouette
- abstract rather than literal
- connected to time, sequence, or structured signal
- compatible in tone with the wordmark

### `TS` direction
- layered horizon
- time window
- waveform restraint
- structured sequence

Avoid literal clocks, arrows, and finance icons.

## 16. Trust, Compliance, and Messaging Rules

### Copy rules
- use plain technical language
- keep claims narrow and supportable
- emphasize decision support, not certainty
- use the product names consistently

### Messaging pattern
Prefer:
- what it is
- who it is for
- how it works at a high level
- what to do next

Avoid:
- visionary manifesto copy
- broad market claims
- unexplained model jargon
- sales language that sounds like performance guarantees

### Sample copy tone
Strong:
- Foundation models for time-series forecasting.
- Visual forecasts for users who want fast market context.
- API access for builders who want direct integration.
- One company, two product paths.

Weak:
- Unlock the future of predictive intelligence.
- Transform uncertainty into alpha with cutting-edge AI.

### Required trust behaviors
- visible disclaimer links
- responsible-use language on Home, Vista, Platform, and Collie
- no hard performance claims without review
- no sensational market language

### Disclosure placement rule
Disclosures should appear:

- in the footer for global access
- near chart-heavy or forecast-heavy sections where interpretation risk is higher
- on dedicated legal pages for full detail

They should not appear only once at the bottom of the site.

## 17. SEO, Accessibility, and Performance by Design

### SEO
- page titles tied to actual user intent
- strong meta descriptions
- crawlable HTML navigation
- internal links between Home, Vista, Platform, and Collie
- sitemap and structured data where relevant

### Accessibility
- semantic heading order
- visible keyboard focus
- high-contrast text
- accessible forms
- alt text for diagrams and screenshots
- no information conveyed by color alone

### Performance
- compressed images
- few font files
- static-first architecture
- motion that degrades cleanly

These are not implementation extras. They are part of the brand impression.

## 18. Responsive Behavior Rules

### Requirement
All key pages must work well on both desktop and mobile in the first shipped version.

### Mobile
- stack hero content before visual
- convert product split cards into full-width panels
- keep CTA labels short
- preserve trust content near the conversion path

### Tablet
- maintain split layouts only when both columns remain readable
- keep screenshots large enough to communicate product shape

### Desktop
- use width and whitespace to establish authority
- avoid filling space with decorative elements

### Universal rule
The information hierarchy must stay the same across breakpoints even when the layout changes.

## 19. Visual Mockup Guardrails

Before accepting any homepage or page mockup, check:

- Does the first screen explain the company clearly?
- Is the Vista / Platform split obvious without reading deeply?
- Is the research / model story integrated without adding confusion?
- Do the visuals support meaning rather than decoration?
- Does the page feel more like a product company than a consultancy?
- Are trust and disclosure cues visible before the footer?
- Would the page still feel strong if animations were removed?
- Are the full product names introduced clearly before shorthand labels appear?
- Is the top-level navigation limited to Products, Company, and Contact?

## 20. Proposed Design Deliverables

### Phase 1: Foundation
- sitemap and nav spec
- homepage wireframe
- visual direction board
- logo direction board
- typography and color system

### Phase 2: Key mockups
- Home
- Vista
- Platform
- Collie
- Company
- Contact

### Phase 3: System
- component library
- responsive rules
- chart and screenshot presentation rules
- trust and disclosure patterns

## 21. Recommended Starting Direction for Execution
Start with the homepage and design system together.

Recommended order:

1. Lock the company narrative and hero language.
2. Lock the Vista / Platform split section.
3. Choose the `Temporis` wordmark and `TS` mark strategy together.
4. Build the color and spacing system.
5. Create Home, Vista, and Platform mockups first.
6. Extend the same system to Collie, Company, and Contact.

## 22. Sources
- Requirements: [requirements.md](requirements.md)
- Nielsen Norman Group, visual hierarchy and design principles: https://www.nngroup.com/articles/principles-visual-design/
- Baymard Institute, readable line length guidance: https://baymard.com/blog/line-length-readability
- web.dev, responsive design basics: https://web.dev/articles/responsive-web-design-basics
- web.dev, accessibility overview: https://web.dev/learn/accessibility
- web.dev, color and contrast: https://web.dev/learn/accessibility/color-contrast
- web.dev, keyboard focus: https://web.dev/learn/accessibility/focus
- OpenAI Business reference: https://openai.com/business/
- Anthropic reference: https://www.anthropic.com/
- Stripe reference: https://stripe.com/

## 23. Final Recommendation
Temporis should not try to look louder than it is. It should look more exact than its peers.

The right brand expression is not "futuristic AI." It is "serious forecasting technology, explained clearly."
