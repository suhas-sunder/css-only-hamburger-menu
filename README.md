# CSS-only hamburger menu

A small, dependency-free demonstration of a hamburger control that opens a sidebar using HTML and CSS. The repository is an **experiment**, not a production-ready navigation component.

## Run it locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser. No installation, build process, or JavaScript is required.
3. Activate the hamburger control to reveal the sidebar; activate it again to hide the sidebar.

## How it works

- A checkbox inside `.burger-menu` stores the open/closed state.
- The `:has(input:checked)` selector changes the bars into an X.
- The adjacent sibling selector `+ .sidebar` moves the sidebar into view.
- Custom properties in `:root` control the bars' dimensions, spacing, colors, and animation.

The sample menu entries are placeholders. Replace them with appropriate navigation links for any real use case.

## Browser support and limitations

The demonstration relies on the CSS `:has()` selector and requires a browser that supports it. The visual control has no explicit accessible name, and the example does not implement production navigation semantics, focus management, or reduced-motion handling. **Do not copy it unchanged into a production site.** Test keyboard and screen-reader interactions, motion preferences, viewport sizes, and the support requirements of your project before adapting it.

## Files

- `index.html` — minimal page markup and placeholder sidebar.
- `styles.css` — checkbox-based control, transitions, and sidebar reveal.

## Verification checklist

- Open the demo in a browser with CSS `:has()` support.
- Toggle the menu using a mouse or touch input.
- Try reaching and toggling the checkbox with a keyboard.
- Check the menu at narrow and wide viewport widths.
- Before production use, add an accessible name, real links, focus behavior, and reduced-motion support.
