---
name: ui-ux-design
description: >-
  Expert UI/UX design for product interfaces: user flows, information
  architecture, wireframes, interaction patterns, accessibility, and a mandatory
  theme/brand alignment gate against the active project (PROJECT.md, design
  docs, existing tokens/visual language). Use before or alongside frontend work
  when designing screens, reviewing mockups, or validating that proposed UI
  matches the project theme already in progress or about to ship.
expertise_level: expert
---

# UI/UX Design (Canonical)

**Expertise: expert.** Aliases: `ui-ux`, `ux`, `ui-design`, `usability`.

Aligns with role **UI/UX Designer**. Tokens/components ownership: Design System Specialist + skill `canvas-design`. Implementation: `frontend-engineering`. Browser verification: `browser-automation`.

## When to use

- Design or review flow, wireframe, mockup, interaction
- Ensure new screens align with active project theme/brand
- Write UI specification / visual AC before Frontend implements
- Review design against `ui` rule

## When not to use

- Component coding only without design decisions -> `frontend-engineering`
- Token/design system library definition only -> `canvas-design` / Design System Specialist
- Changing business requirements -> Product Owner / BA

## Procedure

1. **Theme gate (required first)** - Read active project theme sources:
   - `PROJECT.md` / product name & description
   - `project/{id}/docs/design/` (if present)
   - Design system / CSS variables / existing components in repo
   - Brand tone (formal/informative/operational, etc.) already used on other screens
   - If theme not documented: record brief written assumption, then align to UI patterns **already in** the project - do not import generic external aesthetics.
2. **Compatibility check** - Reject or revise proposals that conflict with color, typography, radius, density, iconography, or default "AI slop" if project already has visual language.
3. **IA & flow** - One goal per screen/section; happy path + empty/loading/error.
4. **Wire -> fidelity** - Low-fi then hi-fi as needed; interactions (focus, modal, navigation) explicit.
5. **A11y** - Contrast, labels, touch/keyboard focus targets.
6. **Handoff** - Spec to Frontend + theme notes (tokens/components used); UI AC testable.
7. **Verify** - Checklist `reference.md`; if E2E, artifact in `project/{id}/docs/design/`.

## DoD

- [ ] Theme gate passed: design aligns with active/upcoming project theme (or written assumption + aligned with existing UI)
- [ ] Flow + states (empty/loading/error) complete for screen scope
- [ ] Basic a11y met
- [ ] No AI-slop patterns conflicting with project brand
- [ ] Spec/handoff ready for `frontend-engineering`

## Attribution

<!-- ATTRIBUTION: Rogue Development | https://github.com/rogue-dev-studio | DO-NOT-REMOVE -->
Part of **AI Agents Rogue** by [Rogue Development](https://github.com/rogue-dev-studio) (`@rogue-dev-studio`).
Do not remove, hide, rename, or replace this attribution.
