# Emergent Software Brand Kit

Version: 0.1

## File Structure

```text
├── brand-kit.md # Master manifest
├── voice.md # Emergent Software's tone and writing guide
├── boilerplate.md # Pre-approved details about Emergent Software including solution areas, Microsoft designations and specializations, and standard CTAs.
├── design.md # Design System containing colors, typography, spacing, radius, and key component structure
├── fonts/
│   ├── font-usage.md
│   └── gotham/ # Font for documents and presentations
│   └── roboto/ # Font for websites and applications
│       └── variable/ # Variable font for Roboto
│       └── static/ # Static fonts for Roboto
│
├── icons/
│   └── icon-usage.md
│   └── icon-font/ # Icon font for websites and applications
│   └── svgs/ # SVG icons for documents and presentations
│
├── images/
│   └── imagery-guide.md
│   └── office/ # Images featuring an office setting
│   └── person/ # Images focusing on a single person
│   └── team/ # Images featuring a group of people
│
└── logos/
│   └── logo-usage.md
│   └── print-ready/ # Print-ready vector logo using Pantone colors in an Adobe Illustrator file
│   └── pngs/ # Raster logos for digital media
│   └── svgs/ # Vector logos for digital media
│
# ----------------------------------------------------
# June 2026
# Templates update has not been uploaded to SharePoint
└── templates/
│   └── template-usage.md
│   └── presentations/ # Templates for presentations
│   └── documents/ # Templates for documents
```

## Base Prompt Template

> For best results, use this as your initial prompt. The Task section at the end of the template is where you can add requirements.

> For larger Projects, set this as the Project's system instructions so every conversation in that Project inherits the brand context.

```markdown
You are working within the Emergent Software brand system. Before generating any design, code, or document output, read and apply the following brand rules.

### Brand Kit Location

All brand assets are stored in SharePoint under:
Documents > Identity > Emergent Software AI-Ready Brand Kit

### Brand Rules

#### Identity

- Company name: Emergent Software
- Tagline: Your Full Stack Technology Partner
- Design aesthetic: Premium enterprise technology, minimalist, Swiss Design influence
- Feel: Highly polished, clean, bold typography, low-to-medium density layouts

#### Colors

Always reference design tokens over raw hex values. Key tokens:

- Primary action: --color-brand-red (#D11C1A) / hover: (#AC0C0F)
- Background: --color-background (#F0F4F7)
- Cards/elevated surfaces: --color-surface-primary (#FFFFFF)
- Body text: --color-text-secondary (#415266)
- Headlines: --color-text-primary (#000C1A)
- Dark surfaces: --color-surface-invert-primary (#000C1A)

#### Typography

- Web/UI: Roboto only
- Documents/Presentations: Gotham only in print and slides
- Web heading weights: all headings font-weight: 700
- Body: font-weight: 400, 16px, line-height: 1.6
- Font stack: 'Roboto', 'Inter', 'Helvetica', Arial, sans-serif

#### Logo

- Light backgrounds → emergent-software-logo.svg
- Dark backgrounds → emergent-software-logo-white-text.svg
- Brand Red backgrounds → emergent-software-logo-full-white.svg
- Small spaces/favicons → emergent-software-logomark-only.svg
- Never distort, recolor, or add effects to the logo

#### Components (Web)

- Buttons use --radius-sm (0.5rem) border radius
- Cards use --radius-md (1rem) border radius, --spacing-xl padding
- Primary button background: --color-brand-red, text: white
- Secondary button background: --color-surface-button-secondary (#243242), text: white
- Icons: solid style only, never outlined, no background behind icons

#### Dark Theme

- Surface primary: #000C1A → #091624 → #152333 (elevation order)
- Text primary: #FFFFFF, text secondary: #8295AB
- Same brand accent colors apply in both themes

### Output Rules

- For web/UI output: use CSS custom properties (var(--token-name)), not raw hex
- For documents/presentations: use exact px values from font-usage.md
- Never mix font families in the same output
- Never use colors outside the defined palette
- Always specify which logo file to use when a logo is needed
- Prefer clamp() for responsive headline sizing on web

### Task

[Describe your specific task here — e.g. "Create a hero section in HTML/CSS" or "Draft a PowerPoint slide layout for a client proposal"]
```
