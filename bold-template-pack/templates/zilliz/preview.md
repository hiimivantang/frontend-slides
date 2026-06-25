# Zilliz Brand Preview Card

Use this small file for title-slide previews only. For final deck generation, read the full design doc listed below.

## Files

- Full design doc: `bold-template-pack/templates/zilliz/design.md`
- Preview card: `bold-template-pack/templates/zilliz/preview.md`

## Selection Metadata

- Slug: `zilliz`
- Tagline: Official Zilliz brand: near-black canvas with the signature sky→blue→purple→berry gradient, Inter + IBM Plex Mono, luminous and technical.
- Mood: modern, technical, confident, luminous, on-brand
- Tone: precise, gradient-forward, engineering, premium
- Formality: medium-high
- Density: medium
- Scheme: dark
- Best for: Any Zilliz-branded deck — product launches, technical keynotes, developer-facing talks, investor updates, and internal Zilliz communications. The default choice whenever the deck must read as official Zilliz, with the brand gradient and vector-database register front and center.
- Avoid for: Non-Zilliz brand work, or contexts that need a warm/light/print register — the dark gradient-forward system is committed to the Zilliz identity.

## Visual Snapshot

The official Zilliz design system: a near-black canvas (#000000) lit by the signature Zilliz brand gradient that flows sky blue (#49BCFF) → blue (#175FFF) → purple (#7F47FF) → berry (#C84CFF). Solid Zilliz Blue carries non-gradient accents; the gradient carries the hero moments — one gradient-clipped hero phrase, large metric values, the 60×4 accent line, bar fills, and the bottom progress bar. Inter sets every headline and body line; IBM Plex Mono handles eyebrows, labels, code, and chrome to signal the vector-database register. Cards are translucent white at 4% with hairline borders; the black canvas gains luminous depth from blurred gradient glow orbs and abstract "vector coordinate" diagonal-line decoration — never a recreated Zilliz logo.

## Preview Ingredients

- Palette: bg #000000; primary/Zilliz Blue #175FFF; navy #061982; sky #49BCFF; purple #7F47FF; berry #C84CFF; green #00DCC6; text #FFFFFF; text-muted #A9B0C0
- Gradient: linear-gradient(135deg, #49BCFF 0%, #175FFF 30%, #7F47FF 65%, #C84CFF 100%)
- Typography: Inter (headlines + body), IBM Plex Mono (eyebrows, labels, code, chrome). See full design doc after selection.
- Signature move: Near-black ground on every surface — luminous, never flat gray.
- Signature move: The Zilliz brand gradient as the single expressive device — one hero phrase, metric values, accent line, bar fills, progress bar.
- Signature move: Inter headlines over sky-blue IBM Plex Mono eyebrows (uppercase, 0.12em tracking).
- Signature move: Translucent white cards (4%) with hairline borders, lifted by blurred gradient glow orbs — no drop shadows.
- Signature move: Abstract vector-coordinate diagonal lines and thin gradient arcs as atmospheric decoration.

## Logo Rule (NON-NEGOTIABLE)

- Never draw, redraw, hand-code (SVG/CSS), or AI-generate the Zilliz logo or star logomark on the preview or any slide. Use only official assets from `https://zilliz.com/brand-assets`, or set the wordmark "Zilliz" in Inter, or omit the mark.
- Never arrange the vector-line decoration to resemble the star logomark.

## International / CJK Preview Note

- If the preview uses Chinese or other CJK text, keep CJK letter-spacing at 0, loosen line-height, and avoid uppercase transforms on CJK runs.
- Use the full `design.md` CJK section after selection for exact font pairings and adjustments.

## Preview Rules

- Build exactly one title slide at 1920x1080 inside the fixed-stage model.
- Preserve the palette, type roles, surface rhythm, gradient discipline, and decorative vocabulary described above.
- Use the user's real title/subtitle/context; do not copy demo slide content.
- The rendered preview must look like a real first slide, not a template-selection card.
- Never place internal workflow text on the slide: no `preview`, `generated from`, `preview.md`, `template`, `preset`, `style option`, `Option A/B/C`, file names, paths, or source-doc labels.
- Never place the template name or slug on the slide itself; mention it only in the chat message.
- Never place user requirement notes such as desired vibe, audience, or internal-use labels on the slide unless the user explicitly wants those exact words in the deck.
- Use only real deck content for visible chrome: deck title, real section title, date, author, company, page number, or genuine content phrases from the user material.
- Do not read `template.html` for preview generation.
- Do not read other templates' `design.md` files.
- After the user picks this template for the full deck, read the full design doc before generating final slides.
