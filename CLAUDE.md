# Robosimu

Static HTML/CSS/JS robotics simulation demos. No build step — edit and refresh.

Run locally: `npx serve .` or `python3 -m http.server`

## Structure

`index.html` — learning path hub
Each demo is a self-contained top-level HTML file (e.g. `arm-kinematics.html`).
`lab/` — demos in progress; not linked from index until ready.

## Design tokens

Dark theme defined in each file's `<style>` block:
- `--bg: #16161a`, `--accent: #d4884a` (warm orange), `--radius: 2px`
- Monospace stack: `'SF Mono', 'Fira Code', 'Cascadia Code', monospace`

Keep tokens consistent across files when adding new demos.
