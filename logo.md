# Logo Agent Documentation Pack

This pack defines a clear three-document system for creating company logos through structured iteration.

The goal is to make logo generation repeatable, reviewable, and easy to refine.

---

# Overall structure

## 1. `requirements.md`
**Purpose:** company-specific brief

This file describes the company and the project.
It should contain the business context, brand intent, constraints, use cases, and project-specific evaluation priorities.

This file answers:
- What company is this?
- What should the logo communicate?
- What constraints must be respected?
- What matters most for this project?

## 2. `design.md`
**Purpose:** general design principles and evaluation policy

This file defines what strong logo design looks like in general.
It should contain enduring best practices, design principles, review standards, and the default scoring rubric.

This file answers:
- What makes a logo good?
- What principles should guide concept creation?
- How should concepts be evaluated?

## 3. `implementation.md`
**Purpose:** execution workflow

This file defines how an agent should read inputs, generate concepts, evaluate them, rank them, and prepare the next iteration.

This file answers:
- How should the work be done?
- What steps should the agent follow?
- What should each run produce?

---

# Separation of concerns

The three files should not overlap unnecessarily.

- `requirements.md` defines **company-specific needs**.
- `design.md` defines **general standards of good logo design**.
- `implementation.md` defines **the process that turns inputs into outputs**.

A simple way to remember the roles:

- `requirements.md` = **what this company needs**
- `design.md` = **what good looks like**
- `implementation.md` = **how to do the work**

---

# `design.md`

## Purpose

`design.md` is the general design-policy document.

It should be reusable across projects and remain mostly stable over time.
It is not the place for company-specific preferences unless they are universal defaults.

## Responsibilities

`design.md` should do two things well:

1. Define the core principles of strong logo design.
2. Define the evaluation framework used to judge concepts.

## What belongs in `design.md`

Include:
- core design principles
- typography principles
- color principles
- shape and form principles
- real-world usability standards
- anti-patterns and common mistakes
- evaluation rubric
- evaluation output format

Do not include:
- company-specific brand attributes
- one-off project constraints
- operational workflow details
- rendering instructions tied to a single company

## Design principles

### Principle 1: Clarity
A strong logo should communicate quickly.
It should be easy to recognize, easy to describe, and easy to remember.

**Implications:**
- Use a limited number of visual elements.
- Avoid unnecessary detail.
- Favor immediate recognition over cleverness for its own sake.

### Principle 2: Distinctiveness
A strong logo should feel ownable.
It should not blend into a sea of generic category symbols.

**Implications:**
- Avoid common visual cliches.
- Build around one memorable idea.
- Check whether the concept is likely to stand out from competitors.

### Principle 3: Brand fit
A strong logo should match the intended perception of the company.
It should feel aligned with the business, audience, and positioning.

**Implications:**
- Let brand attributes influence form and tone.
- Avoid style choices that contradict the business character.
- Prefer strategic relevance over visual novelty.

### Principle 4: Simplicity
A strong logo should reduce the idea to its essential structure.
Simplicity improves recognition, flexibility, and reproduction.

**Implications:**
- Remove decorative noise.
- Use strong shape logic.
- Prefer fewer stronger moves over many weaker ones.

### Principle 5: Scalability
A strong logo should work at very small sizes.
It must remain identifiable in constrained contexts.

**Implications:**
- Test small-size performance early.
- Avoid thin strokes and micro-details.
- Ensure the silhouette remains readable.

### Principle 6: Versatility
A strong logo should work across real applications.
It should not depend on a single perfect presentation context.

**Implications:**
- Test on light and dark backgrounds.
- Test in monochrome.
- Test as full lockup and reduced mark where applicable.

### Principle 7: Meaning
A strong logo should have defensible logic.
It does not need to be literal, but it should be explainable.

**Implications:**
- Tie the concept to the business, audience, or desired impression.
- Prefer intentional symbolism over arbitrary decoration.
- Reject forms that look polished but mean nothing.

### Principle 8: Longevity
A strong logo should survive beyond current visual trends.
It should feel durable rather than momentarily fashionable.

**Implications:**
- Avoid trend-driven effects as the core idea.
- Favor structure over styling tricks.
- Prefer ideas that can age well.

## Acceptable logo types

Concepts may take one or more of these forms:

1. **Wordmark** — logo built primarily from the company name
2. **Lettermark / Monogram** — logo built from initials
3. **Symbol / Icon mark** — standalone symbol
4. **Combination mark** — symbol paired with a wordmark
5. **Emblem** — enclosed badge-style form, used selectively

## Typography principles

Typography should serve both function and personality.

### Guidance
- Prioritize legibility.
- Match type character to brand tone.
- Adjust spacing and proportions intentionally.
- Avoid novelty unless the brief clearly calls for it.

### Evaluation questions
- Is the name easy to read quickly?
- Does the type style align with brand character?
- Does the wordmark still work at small sizes?
- Does the typography feel deliberate rather than default?

## Color principles

Color should strengthen the concept, not carry it.

### Guidance
- Validate the concept in monochrome first.
- Use color to reinforce meaning and recognition.
- Ensure usable light and dark background treatments.
- Avoid relying on color effects to create false complexity.

### Evaluation questions
- Does the logo still work in black and white?
- Does the color direction support the intended brand meaning?
- Is contrast likely to be sufficient in digital use?
- Does the palette feel intentional and ownable?

## Shape and form principles

Shape is often the fastest part of the logo to recognize.

### Guidance
- Favor strong silhouettes.
- Simplify geometry.
- Use symmetry or asymmetry intentionally.
- Keep negative space readable if used.

### Evaluation questions
- Is the silhouette recognizable at a glance?
- Can the form be recalled after a short look?
- Does the structure express the intended qualities?

## Real-world usage standards

Every concept should be evaluated in realistic contexts.

### Required contexts
- website header
- social avatar
- favicon or app icon
- presentation slide
- business card
- monochrome print
- light background
- dark background

### Required variants
- full logo
- monochrome version
- reduced small-size version
- symbol-only version when applicable

## Anti-patterns

Concepts should be rejected or heavily penalized if they rely on:
- visual clutter
- generic industry tropes
- stock-icon logic
- excessive effects
- poor small-size performance
- unexplained symbolism
- weak typography attached to a generic mark
- obvious competitive similarity

## Evaluation framework

This is the default scoring system.

### Core rubric
Score each concept from 1 to 5 on:

1. Brand fit
2. Distinctiveness
3. Clarity
4. Simplicity
5. Memorability
6. Scalability
7. Versatility
8. Typography quality
9. Conceptual meaning
10. Monochrome performance

### Score interpretation
- **45–50**: strong candidate for refinement
- **35–44**: promising but needs targeted improvement
- **25–34**: weak and likely requires major revision
- **below 25**: reject

## Evaluation output format

Each reviewed concept should include:
- concept name
- logo type
- one-sentence concept summary
- visual description
- rationale
- strengths
- weaknesses or risks
- rubric score breakdown
- recommendation: refine, merge, or reject

## Relationship to the other documents

`design.md` is the stable standard.

- `requirements.md` may later add company-specific priorities.
- `implementation.md` should use this document as the source of truth for evaluation.

---

# `implementation.md`

## Purpose

`implementation.md` is the execution document.

It explains how an agent should take `requirements.md` and `design.md`, produce logo concepts, evaluate them, and prepare the next round of iteration.

## Responsibilities

`implementation.md` should define:
- inputs
- outputs
- sequence of steps
- evaluation application
- iteration behavior
- optional agent decomposition

It should not restate general design theory already covered in `design.md`.

## What belongs in `implementation.md`

Include:
- required and optional inputs
- run workflow
- required outputs
- evaluation procedure
- ranking and recommendation procedure
- iteration loop
- runtime contract
- success and failure criteria

Do not include:
- deep design-principle explanations
- company-specific requirements
- long lists of visual best practices already defined in `design.md`

## Inputs

### Required inputs
1. `requirements.md`
2. `design.md`

### Optional inputs
- prior logo attempts
- competitor references
- existing brand assets
- website copy
- color preferences
- banned motifs
- product screenshots
- rendering constraints

## Outputs

A successful run should produce a structured concept package.

### Required outputs
1. **Brief summary**
   - concise summary of the company, task, and constraints
2. **Visual territories**
   - 3 to 5 distinct strategic directions
3. **Logo concepts**
   - one concept per territory
4. **Evaluation**
   - scored review using `design.md`
5. **Recommendation**
   - best candidate and why it wins
6. **Next-step spec**
   - clear refinement or rendering instructions

## Core process

### Step 1: Read the inputs
Read:
- `requirements.md` as the company-specific source of truth
- `design.md` as the general design and evaluation source of truth

### Step 2: Extract the working brief
From `requirements.md`, extract:
- company name
- business category
- offering
- target audience
- brand attributes
- emotional goals
- constraints
- intended usage contexts
- project-specific evaluation priorities

### Step 3: Build a strategy summary
Transform the extracted information into a compact internal brief.

The strategy summary should include:
- brand essence statement
- 3 to 5 core brand attributes
- visual implications of those attributes
- recommended logo type directions
- major constraints and risks

### Step 4: Create visual territories
Generate 3 to 5 meaningfully different territories.
Each territory should differ in strategy, not just surface styling.

Each territory should define:
- intended feeling
- logo type
- form language
- typography direction
- color direction
- central concept anchor

### Step 5: Generate one concept per territory
Each concept should include:
- concept name
- logo type
- one-sentence summary
- visual description
- rationale
- strengths
- risks

### Step 6: Evaluate each concept
Apply the rubric from `design.md`.

If `requirements.md` includes project-specific priorities, use them to interpret the evaluation or influence weighting, while preserving the default rubric structure.

Each concept evaluation should include:
- score by category
- explanation of the score
- biggest weakness
- suggested improvement

### Step 7: Rank and recommend
Rank all concepts.
Identify the strongest 1 to 2 candidates.
Explain:
- why they rank highest
- what should be refined next
- which concepts should be rejected, merged, or revised

### Step 8: Prepare execution-ready output
For the top concept or concepts, produce enough detail to support actual rendering or further design work.

This may include:
- image-generation prompt
- vector construction guidance
- typography guidance
- color guidance
- lockup guidance
- small-size adaptation notes

## Iteration loop

The workflow should support repeated refinement.

### Iteration inputs
- previous concept package
- user feedback
- updated `requirements.md` if needed

### Feedback categories
Feedback should be interpreted in categories such as:
- strategy
- symbol
- typography
- color
- simplicity
- distinctiveness
- usability

### Iteration steps
On each iteration, the agent should:
1. identify what is working
2. identify what needs to change
3. preserve strong elements unless strategy changes
4. revise the targeted aspects
5. re-evaluate the updated concepts
6. explain what changed and why
7. recommend the next iteration step

## Evaluation application rules

To keep evaluation consistent:
- always score every concept
- do not choose a winner before scoring
- do not use vague praise without evidence
- tie comments back to principles in `design.md`
- let company-specific priorities adjust emphasis, not erase the general standards

## Runtime contract

At runtime, the agent should follow this contract:

> Read `requirements.md` as the company-specific brief. Read `design.md` as the general design-policy and evaluation standard. Follow `implementation.md` as the execution workflow. Generate multiple distinct logo directions, explain them, evaluate them, and recommend the best next refinement step.

## Optional multi-agent structure

If the workflow is split across components, use roles like these:

### Agent 1: Brief Interpreter
Input: `requirements.md`
Output: structured working brief

### Agent 2: Concept Generator
Input: working brief + `design.md`
Output: visual territories and concepts

### Agent 3: Evaluator
Input: concepts + `design.md` + project-specific priorities
Output: scored review and recommendation

### Agent 4: Renderer / Prompt Builder
Input: selected concept
Output: rendering instructions

## Single-agent structure

A single agent can run the entire flow using these sections:
1. read inputs
2. build brief
3. create territories
4. generate concepts
5. evaluate concepts
6. rank and recommend
7. prepare rendering guidance

## Success criteria

A run is successful only if:
- at least 3 distinct concepts are generated
- the concepts differ strategically
- each concept ties back to the company brief
- each concept is evaluated consistently
- the output identifies the strongest candidate clearly
- the next action is explicit

## Failure conditions

A run is weak or incomplete if:
- concepts are generic
- concepts are only minor variations
- rationales are vague
- evaluation is inconsistent
- company constraints are ignored
- the chosen winner is unsupported
- rendering guidance is too vague to use

## Relationship to the other documents

`implementation.md` is the operational layer.

- It should use `design.md` for principles and evaluation.
- It should use `requirements.md` for company-specific direction.
- It should not try to replace either document.

---

# Planned next document: `requirements.md`

## Purpose

`requirements.md` will be the company-specific brief.

## What it should contain

It should eventually define:
- company nature
- product or service
- target audience
- brand traits
- desired feeling
- primary logo applications
- competitor context
- constraints
- must-have elements
- must-avoid elements
- project-specific evaluation priorities

## Role in the system

`requirements.md` will complete the three-document system:
- `requirements.md` tells the agent what this company needs
- `design.md` tells the agent how good logo design should be judged
- `implementation.md` tells the agent how to perform the work

