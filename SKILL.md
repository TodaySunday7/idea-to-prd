---
name: idea-to-prd
description: Turn a vague product idea into a Chinese AI-ready PRD through structured questioning, light competitor analysis, MVP scoping, and clear go/no-go judgment. Use when the user wants to clarify a product idea before building, write a PRD for AI coding tools, define target users, narrow MVP scope, or map user flows and requirements.
---

# Idea To PRD

Convert fuzzy ideas into buildable product requirements. Do not jump straight into a PRD.

## When to Activate

- the user wants to write a PRD, product brief, or AI-ready development spec
- the user has a vague or early-stage idea and needs it clarified first
- the user needs help defining target users, MVP scope, user flows, or functional requirements
- the user wants a competitor or substitute scan before deciding whether to build
- the user wants a go/no-go view before investing coding time

## Default Mode

Assume this skill is for:
- Chinese output
- AI-collaboration style documents
- detailed but not bloated PRDs
- lightweight execution, not corporate process theater

Default output directory: `output/`

## Workflow

Always work in this order.

### 1. Clarify the Idea Before Writing

Do not write the PRD until the idea is concrete enough.

Ask targeted questions in small rounds. Prefer 5 to 8 questions per round. Focus on:
- what problem is being solved
- who has the problem
- what the user is doing today instead
- why current solutions are not good enough
- what exact outcome the product should deliver
- what the first version must do
- what does not need to be in version one

If the user is inexperienced, provide concrete examples in the questions instead of abstract product jargon.

### 2. Run a Go / No-Go Filter

Before expanding into a PRD, pressure-test the idea.

Check:
- is there a real user and real workflow
- is the problem frequent enough to matter
- is the pain concrete rather than vague preference
- is there a plausible small MVP
- is the idea meaningfully different from existing alternatives

If the idea looks weak after discussion, say so clearly and stop. Do not force a PRD for a bad idea.

### 3. Do Light but Structured Competitive Analysis

When the product is user-facing or exploratory, analyze current substitutes before scoping the build.

Look for:
- direct competitors
- indirect substitutes
- how users solve this today without a dedicated product
- obvious feature gaps or positioning gaps
- whether the user should still build after seeing the alternatives

Keep it decision-oriented. Avoid long research dumps.

If the question depends on current facts, use current sources and cite them.

### 4. Narrow to a First MVP

Separate:
- must-have for the first usable version
- nice-to-have but not needed now
- explicitly out of scope

Bias toward the smallest testable loop.

### 5. Write the PRD

Only after the above steps are complete, write a Chinese PRD that is suitable for handoff to AI coding tools.

## PRD Structure

Use this default structure unless the user asks for another one:

1. Project Summary
2. Problem Statement
3. Target Users
4. Core Use Cases
5. Competitor and Alternative Snapshot
6. MVP Scope
7. User Flow
8. Functional Requirements
9. Non-Goals
10. Risks and Open Questions
11. Validation Plan
12. Recommended Next Step

## Writing Rules

- Write in Chinese unless the user asks otherwise.
- Prefer clear, operational language over product jargon.
- Distinguish confirmed facts from assumptions.
- Mark unknowns that still need validation.
- Keep scope sharp. Do not let the PRD expand into a wishlist.
- Functional requirements should be concrete enough for AI coding tools to continue.
- User flows should be step-based and readable by non-product people.
- Non-goals are required whenever scope may sprawl.
- If there is not enough information, ask follow-up questions instead of bluffing.

## Output Rules

If the user asks for a saved document, place it under `output/`.

Recommended file naming:
- `YYYY-MM-DD-topic-prd.md`
- use pinyin or simple English slugs

Examples:
- `2026-03-22-water-tracker-miniapp-prd.md`
- `2026-03-22-xiaohongshu-keyword-tool-prd.md`

## Collaboration Style

This skill is mixed-mode by default:
- ask questions first
- gather enough specifics
- then write the PRD

Do not dump a template at the user before understanding the idea.

When the user is new to product work:
- explain tradeoffs plainly
- offer one recommended path when choices appear
- avoid assuming the user knows PM terminology

## Stop Conditions

Stop and say the idea is not worth pursuing yet if:
- no clear user can be identified
- the problem is too weak or too rare
- the value over existing solutions is not clear
- the scope cannot be reduced to a realistic MVP

When stopping, provide a short reason. Do not continue into PRD generation.
