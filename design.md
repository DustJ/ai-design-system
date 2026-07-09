---
version: '0.3'
name: Emergent Software Design System
source_file: Emergent Software Design System
colors:
  background: '#F0F4F7'
  text: '#000C1A'
  primary: '#D11C1A'
  primary-shade: '#AC0C0F'
  brand-red: '#D11C1A'
  brand-red-shade: '#AC0C0F'
  brand-amber: '#F9A825'
  brand-amber-shade: '#ec9a00'
  brand-green: '#00961A'
  brand-green-shade: '#008206'
  brand-blue: '#004192'
  brand-blue-shade: '#002467'
  brand-purple: '#7245CE'
  brand-purple-shade: '#533CA8'
  text-primary: '#000C1A'
  text-secondary: '#415266'
  text-tertiary: '#4D5F73'
  text-link: '#4190EF'
  text-link-shade: '#0072DA'
  text-primary-on-dark: '#FFFFFF'
  text-secondary-on-dark: '#8295AB'
  text-tertiary-on-dark: '#384859'
  surface-background: '#F0F4F7'
  surface-primary: '#FFFFFF'
  surface-secondary: '#F0F4F7'
  surface-tertiary: '#E1E9F0'
  surface-quaternary: '#C5D2E0'
  surface-dark-background: '#000C1A'
  surface-dark-primary: '#091624'
  surface-dark-secondary: '#000C1A'
  surface-dark-tertiary: '#152333'
  surface-dark-quaternary: '#243242'

typography:
  h1:
    fontFamily: Roboto
    fontSize: 62px
    fontWeight: '700'
    lineHeight: 1.15
  h2:
    fontFamily: Roboto
    fontSize: 50px
    fontWeight: '700'
    lineHeight: 1.15
  h3:
    fontFamily: Roboto
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 1.15
  h4:
    fontFamily: Roboto
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 1.15
  h5:
    fontFamily: Roboto
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 1.15
  h6:
    fontFamily: Roboto
    fontSize: 20px
    fontWeight: '700'
    lineHeight: 1.15
  small:
    fontFamily: Roboto
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 1.15
  button:
    fontFamily: Roboto
    fontSize: 16px
    fontWeight: '600'
    lineHeight: 1.3
  paragraph:
    fontFamily: Roboto
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 1.6
  paragraph-article:
    fontFamily: Roboto
    fontSize: 20px
    fontWeight: '400'
    lineHeight: 1.6
  rounded:
    xs: 4px
    sm: 8px
    md: 16px
    lg: 32px
    xl: 64px
    full: 999px
  spacing:
    xxs: 2px
    xs: 4px
    sm: 8px
    md: 12px
    lg: 16px
    xl: 24px
    xxl: 32px
    xxxl: 48px
    section: 64px
  components:
    button-primary:
      backgroundColor: '{colors.primary}'
      padding: 24px 12px
      rounded: '{rounded.small}'
      textColor: '{colors.text-primary-on-dark}'
      typography: '{typography.button}'
    button-primary-hover:
      backgroundColor: '{colors.primary-shade}'
    button-secondary:
      backgroundColor: '{colors.surface-dark-tertiary}'
      padding: 24px 12px
      rounded: '{rounded.small}'
      textColor: '{colors.text-primary-on-dark}'
      typography: '{typography.button}'
    button-secondary-hover:
      backgroundColor: '{colors.surface-dark-secondary}'
    card:
      backgroundColor: '{colors.surface-secondary}'
      padding: '{spacing.xl}'
      rounded: '{rounded.md}'
---

# Emergent Software Design System Guidelines

Version: 0.3

## 1. Aesthetics

Premium enterprise technology with a minimalist style based on Swiss Design. Typography is clean and bold.

### Feel

- Premium
- Highly polished

### Design density

Low to medium density, preferring fewer large modules with strong imagery and terse copy. For data-heavy surfaces, a dense grid-based utilitarian UI is used.

### Visual themes

- Backgrounds are a very light cool-gray leaving white for elevated elements like cards and support surfaces
- Cards and support surfaces are white
- Minimal use of borders

## 2. Colors

### Brand colors

| Token                          | Hex     | Role                                                 |
| ------------------------------ | ------- | ---------------------------------------------------- |
| --color-brand-red              | #D11C1A | Primary action                                       |
| --color-brand-red-shade        | #AC0C0F | Hover state for links and primary action             |
| --color-brand-red-text-on-dark | #EF3A43 | Red text on dark background                          |
| --color-brand-amber            | #F9A825 | Cloud Platform and general-use accent color          |
| --color-brand-amber-shade      | #EC9A00 | Hover state for accent                               |
| --color-brand-green            | #00961A | Software Development and general-use accent color    |
| --color-brand-green-shade      | #008206 | Hover state for accent                               |
| --color-brand-blue             | #004192 | Data & Analytics and general-use accent color        |
| --color-brand-blue-shade       | #002467 | Hover state for accent                               |
| --color-brand-purple           | #7245CE | Artificial Intelligence and general-use accent color |
| --color-brand-purple-shade     | #533CA8 | Hover state for accent                               |

### Light theme

| Token                                  | Hex     | Role                                                                 |
| -------------------------------------- | ------- | -------------------------------------------------------------------- |
| --color-background                     | #F0F4F7 | Background color for main UI                                         |
| --color-surface-primary                | #FFFFFF | Background color for cards and support surfaces                      |
| --color-surface-secondary              | #F0F4F7 | Background color for lightly segmenting sections of copy             |
| --color-surface-segmentation           | #E1E9F0 | Background color segmenting sections of copy                         |
| --color-surface-segmentation-strong    | #C5D2E0 | Background color for heavier segmenting sections of copy             |
| --color-surface-invert-primary         | #000C1A | Dark background color for lowest elevation surface                   |
| --color-surface-invert-secondary       | #091624 | Dark background color for cards and support surfaces                 |
| --color-surface-invert-tertiary        | #0E1C2B | Dark background color segmenting sections of copy                    |
| --color-surface-button-secondary       | #243242 | Dark background color for secondary buttons                          |
| --color-surface-button-secondary-shade | #1F2D3D | Hover state for secondary buttons                                    |
| --color-border-primary                 | #CFDAE5 | Border with low contrast                                             |
| --color-border-secondary               | #ABBDD1 | Border with medium contrast                                          |
| --color-border-invert-primary          | #152333 | Border with low contrast on dark surfaces                            |
| --color-border-invert-secondary        | #2E3C4D | Border with medium contrast on dark surfaces                         |
| --color-text-primary                   | #000C1A | Headlines and important text                                         |
| --color-text-secondary                 | #415266 | Main paragraph copy                                                  |
| --color-text-invert-primary            | #FFFFFF | Headlines and important text on dark surfaces                        |
| --color-text-invert-secondary          | #8295AB | Main paragraph copy on dark surfaces                                 |
| --color-text-on-brand-red              | #FFFFFF | Text that stays white on red surfaces when switching to dark theme   |
| --color-text-on-button-secondary       | #FFFFFF | Text that stays white on button surface when switching to dark theme |
| --color-textlink                       | #4190EF | Text links                                                           |
| --color-textlink-shade                 | #0072DA | Hover state for text links                                           |

### Dark theme

| Token                                             | Hex     | Role                                                                  |
| ------------------------------------------------- | ------- | --------------------------------------------------------------------- |
| --color-dark-theme-background                     | #000C1A | Background color for main UI                                          |
| --color-dark-theme-surface-primary                | #091624 | Background color for cards and support surfaces                       |
| --color-dark-theme-surface-secondary              | #000C1A | Background color for lightly segmenting sections of copy              |
| --color-dark-theme-surface-segmentation           | #152333 | Background color segmenting sections of copy                          |
| --color-dark-theme-surface-segmentation-strong    | #243242 | Background color for heavier segmenting sections of copy              |
| --color-dark-theme-surface-invert-primary         | #F0F4F7 | Light background color for lowest elevation surface                   |
| --color-dark-theme-surface-invert-secondary       | #FFFFFF | Light background color for cards and support surfaces                 |
| --color-dark-theme-surface-invert-tertiary        | #E1E9F0 | Light background color segmenting sections of copy                    |
| --color-dark-theme-surface-button-secondary       | #415266 | Light background color for secondary buttons                          |
| --color-dark-theme-surface-button-secondary-shade | #384859 | Hover state for secondary buttons                                     |
| --color-dark-theme-border-primary                 | #152333 | Border with low contrast                                              |
| --color-dark-theme-border-secondary               | #2E3C4D | Border with medium contrast                                           |
| --color-dark-theme-border-invert-primary          | #D8E1EB | Border with low contrast on light surfaces                            |
| --color-dark-theme-border-invert-secondary        | #ABBDD1 | Border with medium contrast on light surfaces                         |
| --color-dark-theme-text-primary                   | #FFFFFF | Headlines and important text                                          |
| --color-dark-theme-text-secondary                 | #8295AB | Main paragraph copy                                                   |
| --color-dark-theme-text-invert-primary            | #000C1A | Headlines and important text on light surfaces                        |
| --color-dark-theme-text-invert-secondary          | #415266 | Main paragraph copy on light surfaces                                 |
| --color-dark-theme-text-on-brand-red              | #FFFFFF | Text that stays white on red surfaces when switching to light theme   |
| --color-dark-theme-text-on-button-secondary       | #FFFFFF | Text that stays white on button surface when switching to light theme |
| --color-dark-theme-textlink                       | #4190EF | Text links                                                            |
| --color-dark-theme-textlink-shade                 | #0072DA | Hover state for text links                                            |

## 3. Typography

### Font Stack

```css
--font-family: 'Roboto', 'Inter', 'Helvetica', Arial, sans-serif;
```

### Type Scale

Major-Third scale, **16px** root

| Element           | Size  | Weight | Line Height | Color (Light theme / Dark theme)             |
| ----------------- | ----- | ------ | ----------- | -------------------------------------------- |
| H1                | 3.875 | 700    | 1.15        | `--color-text-primary (#000C1A / #FFFFFF)`   |
| H2                | 3.125 | 700    | 1.15        | `--color-text-primary (#000C1A / #FFFFFF)`   |
| H3                | 2.5   | 700    | 1.15        | `--color-text-primary (#000C1A / #FFFFFF)`   |
| H4                | 2     | 700    | 1.15        | `--color-text-primary (#000C1A / #FFFFFF)`   |
| H5                | 1.5   | 700    | 1.15        | `--color-text-primary (#000C1A / #FFFFFF)`   |
| H6                | 1.25  | 700    | 1.15        | `--color-text-primary (#000C1A / #FFFFFF)`   |
| small             | 0.75  | 700    | 1.15        | `--color-text-primary (#000C1A / #FFFFFF)`   |
| paragraph         | 1     | 400    | 1.6         | `--color-text-secondary (#415266 / #8295AB)` |
| paragraph-article | 1.25  | 400    | 1.6         | `--color-text-secondary (#415266 / #8295AB)` |

### Responsive Headlines

Smaller headings on mobile that scale up to large headings on desktop

| Element | clamp                                                     |
| ------- | --------------------------------------------------------- |
| h1      | font-size: clamp(3rem, 2.5459rem + 1.8164vw, 3.875rem)    |
| h2      | font-size: clamp(2.25rem, 1.9094rem + 1.3623vw, 3.125rem) |
| h3      | font-size: clamp(1.875rem, 1.5912rem + 1.1352vw, 2.5rem)  |
| h4      | font-size: clamp(1.5rem, 1.273rem + 0.9082vw, 2rem)       |
| h5      | font-size: clamp(1.25rem, 1.0608rem + 0.7568vw, 1.5rem)   |
| h6      | font-size: clamp(1.125rem, 0.9547rem + 0.6811vw, 1.25rem) |

## 4. Layout

### Spacing Scale

| Token             | Value    |
| ----------------- | -------- |
| --spacing-xxs     | 0.125rem |
| --spacing-xs      | 0.25rem  |
| --spacing-sm      | 0.5rem   |
| --spacing-md      | 0.75rem  |
| --spacing-lg      | 1rem     |
| --spacing-xl      | 1.5rem   |
| --spacing-xxl     | 2rem     |
| --spacing-xxxl    | 3rem     |
| --spacing-section | 4rem     |

### Radius Scale

| Token       | Value   | Use                       |
| ----------- | ------- | ------------------------- |
| --radius-xs | 0.25rem | Dense UIs like data grids |
| --radius-sm | 0.5rem  | Buttons                   |
| --radius-md | 1rem    | Cards                     |
| --radius-lg | 1.5rem  | Wrapper elements          |
| --radius-xl | 2rem    | Rows and sections         |

## 5. Iconography

- Use solid icons not outlined icons
- Icons use brand colors
- Icons should stand on their own and not have an additional background color behind them

## 6. Components

### Buttons

```css
.button--primary {
  background: var(--color-brand-red);
  border-radius: var(--radius-sm);
  border: 1px solid transparent;
  color: var(--color-text-on-brand-red);
  cursor: pointer;
  font-size: 1rem;
  font-weight: 600;
  line-height: 1.3;
  padding-block: 0.75rem;
  padding-inline: 1.5rem;
  text-decoration: none;
  transition: background 0.2s ease-in-out;
}
.button--primary:hover {
  background: var(--color-brand-red-shade);
}

.button--secondary {
  background: var(--color-surface-button-secondary);
  border-radius: var(--radius-sm);
  border: 1px solid transparent;
  color: var(--color-text-on-button-secondary);
  cursor: pointer;
  font-size: 1rem;
  font-weight: 600;
  line-height: 1.3;
  padding-block: 0.75rem;
  padding-inline: 1.5rem;
  text-decoration: none;
  transition: background 0.2s ease-in-out;
}
.button--secondary:hover {
  background: var(--color-surface-button-secondary-shade);
}
```

### Cards

```css
.card {
  background: var(--color-surface-secondary);
  border-radius: var(--radius-md);
  padding: var(--spacing-xl);
}
```
