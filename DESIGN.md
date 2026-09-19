# DESIGN.md — BGS4WHO

Style direction for the Budi Gunadi Sadikin WHO Director-General campaign site (`index.html`).

Source: transcribed from the campaign's own published site and poster assets. The identity is the
owner's, not the agent's. Nothing here invents new brand content.

Dial: **ENERGY 2 / RHYTHM 2 / MOTION 1**

Design Read: candidate campaign landing for WHO Member State delegations and press, in a formal
institutional navy and gold language, dial ENERGY 2 / RHYTHM 2 / MOTION 1.

## Identity

- Personality: institutional, calm, credible, human. A government and multilateral register, not a
  startup register.
- One focal point per screen. On the hero it is the headline "Healthy Long Lives for All."

## Palette (R-29)

Two core colours plus one accent, over neutrals.

| Token | Value | Role |
|---|---|---|
| `--navy` | `#002f5f` | Core. Primary surface, dark sections, footer base. |
| `--blue` | `#0b5fa5` | Core. Links, eyebrows, statistic values. |
| `--sky` | `#dff3fb` | Tint of the core navy family. Section wash. |
| `--gold` | `#f2c14e` | Accent. Used once per screen at the key moment: the headline's second line, the pillar top edge, focus rings. |
| neutrals | `#12202f`, `#5d6a77`, `#d9e2ea`, `#fff` | Text, muted text, hairlines, paper. |

Reason: navy and blue are one hue family, so the page reads as a single colour with a gold accent,
not as four competing colours. Gold appears sparingly so it stays an accent.

## Typography (R-06)

Google Fonts. The page is set in a single family, **Figtree** (`wght@300..900`), for both display
and text, fallback `ui-sans-serif, system-ui, ...`.

- Reason: Figtree is a geometric-humanist sans with a tall x-height, open apertures and a variable
  weight axis (300-900) that covers every weight the stylesheet uses (400 body, 650 nav, 700
  headings, 750 button, 800 eyebrow, 900 brand). One family means the page reads as a single system:
  hierarchy comes from size, weight and the navy/gold palette, not from a second typeface.
- It is not one of the model-default picks (Inter, Geist, Space Grotesk, DM Sans, Poppins,
  Montserrat, Playfair Display), so the page does not read as generated at a glance.
- Tradeoff, stated honestly: an all-sans setting gives up the high-contrast serif echo of the
  campaign poster that a display serif would carry. The register becomes cleaner and more modern,
  less literary; the campaign's gravitas now rests on scale, the navy field and the gold accent.
- Headings are 700, body 400; no monospace, no wide-tracked uppercase display type.
- Served from the Google Fonts CDN with `display=swap`; system fallbacks remain in the stack, so the
  page still renders if the CDN is unreachable.

## Layout (R-31)

- The hero is a full-bleed campaign poster under a dark scrim. Reason: the poster is the campaign's
  primary asset, and the scrim exists to hold text contrast, not for decoration.
- Sections alternate composition (two-column record, dark card band, image band, two-column CV) so
  the page has RHYTHM 2: mostly consistent with deliberate breaks, not one repeated template.
- Spacing is a single generous scale (95px section rhythm, tightened at breakpoints). Reason:
  institutional calm; the page should not feel busy.

## Cards (R-14)

The four leadership cards and the three vision pillars are co-equal by the campaign's own framing
("Four qualities for the next WHO", the Build/Grow/Scale pillars). There is no content hierarchy to
express, so equal cards are content-driven, not a template default. No artificial size variation was
introduced.

## Motion (R-19)

MOTION 1. Hover states and `scroll-behavior: smooth` only. No entrance animations, no loops. Reason:
the audience is delegations and press reading a policy document; motion would add noise.

## Accessibility decisions

- Hero text sits on a scrim whose alpha is kept high across the whole text region, and switches to a
  vertical scrim below 900px so the poster stays visible only below the text (R-25).
- Focus is shown with a gold outline plus a navy halo, so it stays visible on both the light and the
  dark surfaces (R-32).
