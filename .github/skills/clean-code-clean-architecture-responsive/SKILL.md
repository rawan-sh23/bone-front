---
name: clean-code-clean-architecture-responsive
description: Apply the Bone Front standards when building or changing website interfaces, including Arabic and English localization, light and dark themes, logo-led branding, clean architecture, and responsive design.
---

# Clean Code, Clean Architecture, and Responsive UI

Apply these standards to website work in this repository:

## Arabic and English

- Support both Arabic and English in user-facing interfaces.
- Keep translated strings in locale resources rather than embedding text in components.
- Provide a clear language switch and use the selected language consistently across the interface.
- Set the document language and text direction for the active locale: Arabic uses RTL, English uses LTR.
- Ensure layouts, icons, navigation, and form controls remain usable in both directions; do not assume that mirroring every element is correct.
- Use the project's existing localization conventions where available. If none exist, choose a small, maintainable approach appropriate to the app rather than adding an unnecessary framework.

## Light and dark themes

- Provide an accessible theme control that lets users switch between light and dark.
- Use shared design tokens (for example, CSS custom properties) so components do not hardcode theme colors.
- Keep the selected theme consistent across navigation and reloads, following existing app conventions.
- Maintain readable contrast, visible focus states, and appropriate colors for both themes.

## Logo-led brand styling

- Inspect the supplied logo and existing brand assets before choosing primary colors or visual treatments.
- Derive the primary palette and supporting accents from the logo; use shared tokens consistently across components.
- Preserve the logo asset and its proportions. Do not invent a replacement mark or guess brand colors when the asset is unavailable; ask for the logo or brand guidance when needed.
- Keep brand styling coherent across pages, prompts, and reusable UI elements without sacrificing legibility or accessibility.

## Clean code and architecture

- Follow the repository's existing framework, naming, formatting, and architectural conventions.
- Keep components focused, reusable where appropriate, and separated from translation data, theme tokens, and domain logic.
- Prefer simple, explicit implementations over unnecessary abstractions or dependencies.
- Preserve existing behavior and update directly related documentation and tests when behavior changes.

## Responsive and accessible behavior

- Design mobile-first and verify layouts at narrow, medium, and wide viewport sizes.
- Prevent horizontal overflow and keep navigation, content, and controls usable on touch screens.
- Use semantic HTML, keyboard-operable controls, accessible names, and visible focus indicators.
- Validate both locales and both themes at representative viewport sizes.
