---
name: Sakura Browser Desktop
colors:
  surface: '#f9f9ff'
  surface-dim: '#d9d9e0'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3fa'
  surface-container: '#ededf4'
  surface-container-high: '#e8e7ef'
  surface-container-highest: '#e2e2e9'
  on-surface: '#1a1b21'
  on-surface-variant: '#564147'
  inverse-surface: '#2e3036'
  inverse-on-surface: '#f0f0f7'
  outline: '#897177'
  outline-variant: '#dcbfc6'
  surface-tint: '#a63260'
  primary: '#962554'
  on-primary: '#ffffff'
  primary-container: '#b63e6c'
  on-primary-container: '#ffe5eb'
  inverse-primary: '#ffb1c7'
  secondary: '#884c64'
  on-secondary: '#ffffff'
  secondary-container: '#fdb1cd'
  on-secondary-container: '#7a4058'
  tertiary: '#585055'
  on-tertiary: '#ffffff'
  tertiary-container: '#71686d'
  on-tertiary-container: '#f5e9ef'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffd9e2'
  primary-fixed-dim: '#ffb1c7'
  on-primary-fixed: '#3f001c'
  on-primary-fixed-variant: '#871748'
  secondary-fixed: '#ffd9e5'
  secondary-fixed-dim: '#fdb1cd'
  on-secondary-fixed: '#380920'
  on-secondary-fixed-variant: '#6c344c'
  tertiary-fixed: '#ecdfe5'
  tertiary-fixed-dim: '#cfc3c9'
  on-tertiary-fixed: '#201a1e'
  on-tertiary-fixed-variant: '#4c4549'
  background: '#f9f9ff'
  on-background: '#1a1b21'
  surface-variant: '#e2e2e9'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.015em
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
    letterSpacing: -0.012em
  headline-sm:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '600'
    lineHeight: 24px
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '400'
    lineHeight: 22px
    letterSpacing: -0.005em
  body-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
    letterSpacing: 0em
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
    letterSpacing: 0.005em
  label-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '500'
    lineHeight: 18px
    letterSpacing: 0em
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 14px
    letterSpacing: 0.01em
  code-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
    letterSpacing: 0em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 0.5rem
  margin: 0.75rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 0.75rem
  space-lg: 1rem
  space-xl: 1.5rem
---

## Brand & Style
The design system establishes a focused, hyper-refined desktop browser experience balancing lightweight tactile minimalism with deliberate floral warmth. The design style combines modern OS-native desktop utility with crisp, architectural surface layering. 

The aesthetic is precise, unencumbered, and rapid. Atmospheric accents provide warmth and orientation without degrading legibility or viewport focus. Visual weight favors content rendering first: chromes, side panels, and toolbars maintain quiet structural clarity, while interactive cherry blossom pinks mark navigational states, pinned tabs, and security clearances.

## Colors
Color tokens are strictly paired across light and dark modes to enforce contrast safety and legibility standards.

### Light Mode
- **Canvas / Background**: `#F7F8FA`
- **Surface**: `#FFFFFF`
- **Elevated Canvas / Floating Surface**: `#FFFFFF`
- **Subtle Surface Tint**: `#FCEFF5`
- **Border / Divider**: `#E4E6EB`
- **Text Primary**: `#15171C`
- **Text Secondary**: `#68707D`
- **Text Muted / Placeholder**: `#9BA3AF`
- **Accent Primary (Interactive / Text)**: `#B63E6C` (Guarantees WCAG AA 4.5:1+ against light surfaces; never use pastels for text or essential glyphs)
- **Accent Soft Glow / Decorative**: `#F4A9C5`

### Dark Mode
- **Canvas / Background**: `#0E0F12`
- **Surface**: `#17181C`
- **Elevated Canvas / Floating Surface**: `#1F2126`
- **Subtle Surface Tint**: `#2B1A22`
- **Border / Divider**: `#282A30`
- **Text Primary**: `#F2F3F5`
- **Text Secondary**: `#A0A6B2`
- **Text Muted / Placeholder**: `#68707D`
- **Accent Primary (Interactive)**: `#F7BBD4`
- **Accent Secondary (Interactive Alternate / Glow)**: `#E88FB2`
- **Accent Soft Glow / Decorative**: `#E88FB2`

## Typography
Typography relies on `Inter` with fallback to `system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif` for native platform speed, rendering sub-pixel precision across macOS, Windows, and Linux.

The scale is tailored for dense desktop environments:
- **Display / Settings Headers (`headline-lg`, `headline-md`)**: Reserved for application level modals, onboarding panes, and browser settings.
- **Tab Titles, Omnibox, Toolbar Buttons (`body-md`, `label-md`)**: Standard density baseline at 13px with an 18px line height to maintain alignment with 28px/32px input fields and vertical tab strips.
- **Micro-labels, Badges, Keyboard Shortcuts (`label-sm`, `code-sm`)**: 11px and 12px sizes rendered with medium weight to guarantee legibility at small scale.

## Layout & Spacing
The layout follows an immutable 4px spatial rhythm (`4px`, `8px`, `12px`, `16px`, `24px`, `32px`, `40px`, `44px`, `48px`, `64px`).

### Desktop Application Shell
- **App Frame & Titlebar**: 40px fixed height; contains window management controls, integrated tab strip, and sync indicator.
- **Omnibox Toolbar**: 44px fixed height; housing back/forward/reload controls, unified address bar, and extension actions.
- **Vertical Sidebar (Tab & Workspace strip)**: Collapsed state at 48px; expanded state at 240px.
- **Internal Gaps & Padding**:
  - `space-xs` (4px): Micro-gaps between toolbar icon buttons, badge insets, tab close buttons.
  - `space-sm` (8px): Padding within omnibox inputs, vertical padding in menu items, tab gap.
  - `space-md` (12px): Lateral padding of omnibox, lateral spacing in modal headers and list rows.
  - `space-lg` (16px): Content margin inside popovers, side sheets, and settings modules.
  - `space-xl` (24px): Structural padding for onboarding, internal browser page containers.

## Elevation & Depth
Elevation is achieved using a dual strategy of low-contrast hairline borders and ambient shadows. Solid planar fills separate the browser chrome from web content without heavy skeuomorphic drop shadows.

- **Level 0 (App Canvas / Chrome Background)**: Flat `#F7F8FA` (Light) / `#0E0F12` (Dark). No shadow.
- **Level 1 (Browser Toolbars, Side Panels, Active Tab Surface)**: Surface `#FFFFFF` (Light) / `#17181C` (Dark), surrounded by a 1px solid border `#E4E6EB` (Light) / `#282A30` (Dark).
- **Level 2 (Dropdowns, Omnibox Autocomplete, Menus)**: Elevated surface `#FFFFFF` (Light) / `#1F2126` (Dark), bordered by `#E4E6EB` / `#282A30`, with ambient shadow:
  - Light mode: `0 4px 16px rgba(0, 0, 0, 0.08)`
  - Dark mode: `0 4px 16px rgba(0, 0, 0, 0.45)`
- **Level 3 (Modal Dialogs, Command Palettes)**: Surface `#FFFFFF` (Light) / `#1F2126` (Dark), 1px border `#E4E6EB` / `#282A30`, with combined key and ambient shadow:
  - Light mode: `0 12px 32px rgba(0, 0, 0, 0.12), 0 2px 6px rgba(0, 0, 0, 0.04)`
  - Dark mode: `0 12px 32px rgba(0, 0, 0, 0.60), 0 2px 6px rgba(0, 0, 0, 0.20)`
- **Focus Rings & Aura Accents**: Focus rings use a 2px offset-free outline with `#B63E6C` in Light Mode and `#F7BBD4` in Dark Mode. Ambient active states leverage decorative soft glows (`#F4A9C5` at 25% opacity in Light Mode, `#E88FB2` at 20% opacity in Dark Mode).

## Shapes
Shapes employ purposeful geometric radiuses tailored for desktop information density:
- **Radius 4px (`radius-xs`)**: Contextual menu items, inner badges, command palette shortcuts, tab audio indicators.
- **Radius 6px (`radius-sm`)**: Standard buttons, omnibox action chips, inputs, vertical tab items.
- **Radius 8px (`radius-md`)**: Omnibox frame, popover cards, modal shells, extension flyouts.
- **Radius 12px (`radius-lg`)**: Floating HUDs, download monitor panels, settings card groups.
- **Full Radius (`radius-full`)**: Circular action buttons, avatar masks, status pills, and counter dots.

## Components

### Buttons
- **Primary**: Filled `#B63E6C` with text `#FFFFFF` (Light); filled `#F7BBD4` with text `#17181C` (Dark). Radius 6px. Height 28px (compact) or 32px (standard). Padding: 0 12px.
- **Secondary / Ghost**: Background transparent; hover background `#FCEFF5` (Light) / `#2B1A22` (Dark). Text `#15171C` (Light) / `#F2F3F5` (Dark). Radius 6px.
- **Icon Actions (Chrome Toolbar)**: 28x28px square, radius 6px. Hover: background `#E4E6EB` at 50% (Light) / `#282A30` (Dark). Pressed: scale 0.98.

### Omnibox & Text Inputs
- Height 32px. Radius 8px.
- Background: `#FFFFFF` (Light) / `#17181C` (Dark) with 1px border `#E4E6EB` / `#282A30`.
- Text: 13px (`body-md`). Placeholder text `#9BA3AF` (Light) / `#68707D` (Dark).
- Focus state: Border color `#B63E6C` (Light) / `#F7BBD4` (Dark), with a 2px outer glow using `#F4A9C5` at 30% alpha (Light) or `#E88FB2` at 25% alpha (Dark).

### Tabs (Horizontal & Vertical)
- **Active Tab**: Surface background (`#FFFFFF` in Light, `#17181C` in Dark) with a bottom or lateral 2px accent indicator (`#B63E6C` in Light, `#F7BBD4` in Dark). Text color `#15171C` (Light) / `#F2F3F5` (Dark), font weight 500.
- **Inactive Tab**: Transparent background. Text `#68707D` (Light) / `#A0A6B2` (Dark). Hover triggers `#FCEFF5` (Light) / `#2B1A22` (Dark) background transition.
- Radius: 6px on container; height 32px (Horizontal) or 36px (Vertical).

### Checkboxes & Radios
- Size: 16x16px. Radius 4px (Checkbox) or Full (Radio).
- Unchecked: 1px border `#E4E6EB` (Light) / `#282A30` (Dark), surface background.
- Checked: Background `#B63E6C` (Light) / `#F7BBD4` (Dark), icon check color `#FFFFFF` (Light) / `#17181C` (Dark).

### Chips & Workspace Badges
- Height 22px, padding 0 8px, radius 4px.
- Tint variant: Background `#FCEFF5` (Light) / `#2B1A22` (Dark), text `#B63E6C` (Light) / `#F7BBD4` (Dark), font size 11px (`label-sm`).

### Cards & Flyout Panels
- Surface `#FFFFFF` (Light) / `#1F2126` (Dark), 1px solid border `#E4E6EB` / `#282A30`, radius 8px or 12px.
- Padding: 12px or 16px. Elevation Level 2.