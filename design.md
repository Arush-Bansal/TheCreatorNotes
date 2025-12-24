# Design Specification: The Hybrid Insight Language

This document defines the visual language for "The Creator Notes," merging **Option 1 (Illustrated Insight)** with constrained **Option 3 (Structured Canvas)** elements.

## Core Visual Primitives

### Color Palette (Vibrant & Warm)
- **Primary Background**: `#FAF9F6` (Warm Off-white/Cream)
- **Primary Text**: `#1A1A1A` (Near Black)
- **Core Accent (The "Hook")**: `#EB0028` (TED Red)
- **Secondary Accents**:
  - `Education Teal`: `#0D9488`
  - `Insight Yellow`: `#FACC15`
  - `Map Indigo`: `#4F46E5`

### Typography
- **Headings**: `Outfit`, Sans-Serif (Bold, friendly, 700+ weight)
- **Body**: `Inter`, Sans-Serif (Clean, high readability)
- **Annotations**: `Permanent Marker` or similar (Hand-drawn feel for insights)

### UI Elements
- **Borders**: 2px solid `#1A1A1A` for cards and sections (Playful bold look).
- **Shadows**: Hard, offset shadows (e.g., `4px 4px 0px #1A1A1A`) to create a 2D-illustration feel.
- **Corners**: Subtle rounding (`var(--radius-sm)`).

---

## Strategy for Hybrid Integration

### The "Illustrated Insight" (Default)
- Use for 95% of the site (Home, Articles, Tools).
- Characterized by vibrant color blocks and hand-drawn SVG accents.
- Focus: **Content Readability**.

### The "Structured Canvas" (Teaching Aid)
- Reserved ONLY for `/start-here` and specific roadmap sections.
- **Rules**:
  - Uses the same color palette as the rest of the site.
  - No "App-like" interactivity (No dragging or tool panels).
  - Uses **SVG Lines and Nodes** to show relationship between ideas.
  - Goal: **Orientation & Hierarchy**.

---

## Components Update Plan

- **Layout**: Switch to light-mode primary.
- **Navbar**: Solid color blocking or thick lower border.
- **Cards**: Switch to "Offset Shadow" style with vibrant category tags.
- **Note Page**: Focus on "Reading Experience." Add `Permanent Marker` style annotations in the margins or as pull quotes.
- **Map Component**: Create a `Roadmap.astro` component that renders a static, structured path using SVG.
