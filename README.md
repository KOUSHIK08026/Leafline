# Leafline

Leafline is a project-based task tracker built as a single HTML file, using a cyan-themed "Crystalline Growth" design system.

## Features
- **Project & Task Management**: Organise work into projects with dedicated task lists.
- **Priority Selection**: Set Low / Medium / High priority on both projects and tasks (defaults to Medium).
- **Horizontal Task Canvas**: Root tasks flow side-by-side for a board-like planning view.
- **Interactive Tree Structure**: Infinite sub-task nesting with visual connector lines.
- **Drag & Drop**: Move tasks between levels or reorder them seamlessly.
- **Glassmorphic Design**: Cyan "Crystalline Growth" theme with smooth animations.
- **Data Persistence**: Offline-first via `localStorage` — no server needed.

## Changelog

*Check this section before every new commit.*

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
