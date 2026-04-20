---
description: Generate UI mockups as ASCII diagrams and Excalidraw JSON
argument-hint: [feature or screen description]
---

# /ai-msdt:mockup

## Goal
Design UI mockups for the described screen or feature — delivered as annotated ASCII wireframes and ready-to-import Excalidraw JSON.

## Instructions

### 1. Understand the context
- Read the codebase to identify the tech stack (React, Angular, Blazor, etc.)
- Find existing layout patterns, navigation structure, and reusable components
- Understand the user flow that leads to and from this screen

### 2. ASCII wireframe
- Draw a full-width ASCII wireframe that shows layout structure
- Use box-drawing characters: `┌─┐ │ └─┘ ├─┤ ╔═╗ ║ ╚═╝`
- Annotate each region with a label: `[NavBar]`, `[Sidebar]`, `[Card]`, `[Button: Submit]`
- Mark interactive elements explicitly: `[Input: email]`, `[Dropdown: role]`, `[Link: forgot password]`
- Show responsive intent: note which panels collapse on mobile

### 3. Component mapping
List which existing components map to each region and what needs to be created:
- `REUSE` — component already exists (include file path)
- `ADAPT` — component exists but needs props/slots change
- `NEW` — component must be created from scratch

### 4. Excalidraw JSON
Generate a valid Excalidraw scene JSON (`{"type":"excalidraw","version":2,"elements":[...],"appState":{...}}`) that:
- Uses rectangles for containers and cards
- Uses text elements for labels and placeholder copy
- Uses arrows for data flow or navigation relationships
- Groups related elements with `groupIds`
- Uses a clean palette: background `#f8f9fa`, primary `#4361ee`, surface `#ffffff`, border `#dee2e6`

Wrap the JSON in a fenced code block tagged `excalidraw` so the user can copy-paste it directly into [excalidraw.com](https://excalidraw.com) via **Open → Paste from clipboard**.

### 5. UX notes
- Call out any accessibility concerns (contrast, keyboard navigation, ARIA roles)
- Flag UX anti-patterns if spotted
- Suggest one improvement the user may not have considered

## Output format
1. **Screen summary** — one paragraph: what this screen does and who uses it
2. **ASCII wireframe** — full layout with annotations
3. **Component map** — REUSE / ADAPT / NEW table
4. **Excalidraw JSON** — fenced ```excalidraw block, ready to import
5. **UX notes** — accessibility, anti-patterns, one unsolicited improvement

## Rules
- Never invent features not described or implied by the codebase
- Wireframe must reflect actual viewport proportions (desktop-first, then note mobile breakpoints)
- Excalidraw JSON must be valid — no trailing commas, all required fields present
- Keep placeholder copy realistic, not "Lorem ipsum"
