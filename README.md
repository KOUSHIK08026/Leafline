# Leafline

Leafline is a project-based task tracker built as a single HTML file, using a cyan-themed "Crystalline Growth" design system.

## Features
- **Project & Task Management**: Organise work into projects with dedicated task lists.
- **Priority Selection**: Set Low / Medium / High priority on both projects and tasks (defaults to Medium).
- **Dark / Light Theme**: One-click theme toggle in the header; preference persists across sessions.
- **Animated Task Completion**: SVG checkmark dot with a spring pop animation and stroke draw-in on every toggle.
- **Horizontal Task Canvas**: Root tasks flow side-by-side for a board-like planning view.
- **Interactive Tree Structure**: Infinite sub-task nesting with visual connector lines.
- **Drag & Drop**: Move tasks between levels or reorder them seamlessly.
- **Glassmorphic Design**: Cyan "Crystalline Growth" theme with smooth animations.
- **Data Persistence**: Offline-first via `localStorage` — no server needed.

## Changelog

*Check this section before every new commit.*

### [1.0.3] - 27-04-2026
- **Dark / Light Theme Toggle:** Added a 🌙/☀️ toggle button in the top-right header area.
- **Full Dark Mode:** All surfaces, cards, modals, badges, tree connectors, and form controls styled for dark mode.
- **Theme Persistence:** Selected theme saved to `localStorage` and restored on next load.
- **Animated Task Checkmark:** Replaced the plain status dot with an SVG circle + checkmark; unchecked state shows a hollow outlined circle, checked state fills it with a white ✓ inside.
- **Spring Pop Animation:** Toggling a task plays a scale `1 → 0.75 → 1.15 → 1` spring pop (350ms, cubic-bezier spring curve).
- **Checkmark Draw-in:** The ✓ strokes in via `stroke-dashoffset` after the fill appears (~120ms delay, 200ms duration).
- **Card Click-to-Toggle:** Clicking anywhere on a task card body marks it done/undone — mirrors the status dot. Action buttons (+, ✏️, 🗑️) and the expand/collapse toggle are excluded via `stopPropagation`.
- **Completion Visual Feedback:** Completed cards get a strikethrough on the task title and reduced opacity (0.72 light / 0.65 dark) so done tasks are visually distinct from active ones.


### [1.0.2] - 26-04-2026
- **Project Priority:** Added a Priority field (Low / Medium / High, defaulting to Medium) to the New Project and Edit Project modal, displayed side-by-side with Due Date — matching the task modal layout.
- **Priority Persistence:** Priority is now saved and restored correctly when editing an existing project.

### [1.0.1] - 23-04-2026
- **Horizontal Task Canvas:** Root tasks now display horizontally for a "Progress Board" view; nested sub-tasks remain vertical.
- **Synchronized UI:** Sidebar and main content transitions are hardware-accelerated and synced at 250ms.
- **Fixed Branding:** "Leafline" header stays stationary next to the toggle button regardless of sidebar state.
- **Zero-Shift Toggle:** Hamburger menu is fixed to a global coordinate — no jumping during transitions.
- **Visual Polish:** Eliminated ghost icon fragments and layout gaps during sidebar transitions.
- **Scroll:** Horizontal scroll support added for projects with many root tasks.

### [1.0.0] - 21-04-2026
- **Initial Release:**
  - Created the single-file structure (`Leafline.html`).
  - Implemented the "Crystalline Growth" cyan-themed design system.
  - Added drag-and-drop support for the task tree.
  - Added basic creation, editing, and deletion of projects and tasks.
  - Integrated `localStorage` persistence.
