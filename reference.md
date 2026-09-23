# UI/UX Design - Reference (Expert)

## Theme / brand alignment gate (blocker)

Before wireframes or mockups are finalized, answer every point:

| # | Question | Pass if |
|---|------------|------------|
| 1 | Which active project? (`PROJECT.md` / `project/{id}/`) | Product identity is clear |
| 2 | What visual theme already exists? (colors, fonts, density, components) | Referenced from design docs **or** existing UI in the repo |
| 3 | Does the proposal use the same tokens/patterns? | Yes, or there is a written rationale + design approval |
| 4 | Can the proposal be recognized as the same product without reading the nav label? | Brand/theme is strong and consistent |
| 5 | Does it avoid generic templates (hero clutter, pill cluster, purple-gradient default, etc.) when the project already has direction? | Yes |

**Fail theme gate** -> do not hand off to Frontend; revise first.

Theme sources (priority order):

1. Project design system / tokens (`docs/design/`, stylesheet variables, component library)
2. Existing screens/modules in the frontend codebase
3. SRS / UI requirements that mention brand or tone
4. Written assumptions in `docs/design/` (only if 1-3 are empty)

## Screen checklist

- [ ] One clear goal per screen/section
- [ ] Empty / loading / error / success states
- [ ] Hierarchy: brand/product is not overshadowed by generic headlines (when the surface is branded)
- [ ] Mobile-first or responsive per rule `ui`
- [ ] Modal/overlay: does not break layout behind; focus is managed
- [ ] Cards only as interaction containers (aligned with rule `ui`)

## Handoff to Frontend

- Components/tokens that must be used
- Spacing/type scale if not yet in the design system
- Theme note: "aligned with module X / token Y"
- Verifiable UI AC (`browser-automation` or manual)

## Anti-patterns

- Replacing the project theme with a new visual trend without ADR/design approval
- Mixing two densities/typographies without a system
- Excessive sticker/badge overlays on primary media
- Designs that look good on desktop only and break on mobile
