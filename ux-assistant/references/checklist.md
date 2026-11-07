# UX Assistant checklist

Fixed checks to run before any judgement calls. Each has an ID so findings can cite it. Measure whenever you have values.

## A · Accessibility (WCAG 2.2 AA)
- **A-01 Text contrast**: body text ≥ 4.5:1; large text (≥ 24 px, or ≥ 18.66 px bold) ≥ 3:1. Compute with relative luminance; include text on images and on hover/focus states.
- **A-02 Non-text contrast**: input borders, icons that carry meaning and focus rings ≥ 3:1 against their background.
- **A-03 Colour not alone**: status, errors and links are not signalled by colour only (add icon, text or underline).
- **A-04 Labels**: every input has a programmatic label; placeholders are not labels.
- **A-05 Names**: icon-only buttons and links have an accessible name (aria-label or visually hidden text).
- **A-06 Images**: informative images have alt text; decorative ones have `alt=""`.
- **A-07 Headings**: one h1; levels don't skip; headings describe their section.
- **A-08 Landmarks**: main, nav and footer present; skip link on long pages.
- **A-09 Keyboard**: every interactive element is reachable and operable by keyboard, in a logical order, with no trap.
- **A-10 Focus visible**: a visible focus indicator on every focusable element (2.4.7), not hidden by sticky elements (2.4.11).
- **A-11 Target size**: pointer targets ≥ 24 × 24 px (2.5.8); aim for 44 × 44 on touch.
- **A-12 Motion**: animations respect `prefers-reduced-motion`; nothing flashes more than 3 times a second.
- **A-13 Language**: `<html lang>` set.
- **A-14 Dialogs**: focus moves into the dialog, is trapped while open, returns to the trigger on close, Esc closes.
- **A-15 Errors**: form errors are announced, describe the fix, and are linked to the field (aria-describedby).
- **A-16 Zoom and reflow**: content works at 200% zoom and 320 px width without horizontal scrolling.

## S · States
- **S-01 Empty**: lists, tables and dashboards have a designed empty state that explains what will appear and how to add it.
- **S-02 Loading**: skeletons or spinners for anything slower than ~300 ms; layout doesn't jump when data arrives.
- **S-03 Error**: network and server errors say what happened and how to recover.
- **S-04 Long content**: long names, emails and translations wrap or truncate with a tooltip, never overflow.
- **S-05 Many items**: pagination, virtualisation or "show more" for long lists.
- **S-06 Disabled**: disabled controls explain why, or are replaced by an explanation.
- **S-07 Success**: actions confirm what happened (toast or inline), with undo for destructive ones.
- **S-08 Overlays**: dropdowns and popovers stay inside the viewport and don't cover the control that opened them or the primary action.

## L · Layout and visual
- **L-01 Spacing scale**: spacing uses a consistent scale (e.g. 4/8 px); flag one-off values.
- **L-02 Alignment**: elements align to shared edges; flag near-misses of 1–3 px.
- **L-03 Hierarchy**: one primary action per view; the primary button is visually distinct from secondary ones.
- **L-04 Type scale**: limited set of sizes; body text ≥ 16 px on mobile for inputs (prevents iOS zoom).
- **L-05 Line length**: body text roughly 45–80 characters per line.
- **L-06 Responsive**: no horizontal scroll at 375 px; touch layouts stack sensibly.
- **L-07 Tokens**: colours, radii and shadows come from tokens; flag raw hex values that duplicate a token.

## C · Content
- **C-01 Button labels**: verbs that say what happens ("Book a demo", not "Submit").
- **C-02 Specific headings**: headings name the content, not "Overview" everywhere.
- **C-03 Plain language**: no internal jargon or system terms in UI copy.
- **C-04 Consistent terms**: the same thing has the same name everywhere.
- **C-05 Error copy**: says what went wrong and how to fix it, without blame or "Oops".

## F · Forms
- **F-01 Autocomplete**: inputs use correct `type` and `autocomplete` values.
- **F-02 Required fields**: marked, and only what the next step truly needs.
- **F-03 Validation timing**: validate on blur or submit, not on every keystroke while the user is still typing.
- **F-04 Input masks**: don't block pasting; accept common formats.
