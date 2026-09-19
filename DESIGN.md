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

Google Fonts, chosen to stay off the model-default roster (Inter, Geist, Space Grotesk, DM Sans,
Poppins, Montserrat, Playfair Display) that makes generated pages read as generated.

- Headings: **Source Serif 4** (`opsz,wght@8..60,200..900`), fallback Georgia, Times New Roman.
  Reason: an Adobe open-source serif with real optical sizes, drawn for reading; its transitional
  forms and sturdy stroke contrast give the institutional gravitas the campaign register needs, and
  they echo the high-contrast serif on the campaign poster.
- Body and UI: **Source Sans 3** (`wght@200..900`), fallback `ui-sans-serif, system-ui, ...`.
  Reason: the humanist companion to Source Serif 4 from the same designer; drawn for interface and
  long-form legibility, neutral enough to defer to the headings, with a variable weight axis that
  covers every weight the stylesheet uses (650, 750, 900).
- The pair is one superfamily, so the page reads as a single typographic system rather than two
  fonts borrowed from different places.
- Both are variable fonts served from the Google Fonts CDN with `display=swap`. System fallbacks
  remain in the stack, so the page still renders if the CDN is unreachable.
- No monospace, no wide-tracked uppercase display type.

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
