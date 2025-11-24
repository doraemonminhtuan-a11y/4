# Copilot Instructions - Web Course Introduction Page

## Project Overview
Educational HTML project showcasing a basic web programming course curriculum. Single-file HTML document with embedded CSS styling for a course landing/introduction page in Vietnamese.

## Key Files & Purpose
- **`exercise1_beforecss.html`** - Main deliverable; contains HTML structure + inline CSS styling for course information display. Includes course overview, schedule table, prerequisites, and signup links.

## Architecture & Structure
This is a **single-page, self-contained HTML document** with:
- **HTML structure**: Semantic layout with main content wrapper (`#main-content`)
- **CSS styling**: All styles embedded in `<style>` tags; centered design with max-width of 800px
- **Assets**: References two image files (HTML5_logo.png, OIP.webp) - ensure these exist in the root directory
- **Language**: Vietnamese (lang="vi") - content is in Vietnamese

## Common Patterns & Conventions

### Styling Approach
- **Centered layout**: Uses `max-width: 800px; margin: 0 auto` for container centering
- **ID-based selectors**: Heavy use of `#main-content` prefix for all content styling (allows easy page-wide styling changes)
- **Responsive images**: Images use `max-width: 200px; height: auto` for scaling

### Content Structure
- Course information sections use `<h2>` for major sections (Nội dung, Yêu cầu, Lịch học)
- Lists use `display: inline-block` with custom text-alignment
- Tables styled with explicit borders and padding
- Links styled with custom color (`#d9534f`) and hover effects

## Development & Testing
- **Debug/Preview**: VS Code launch configuration (`launch.json`) opens file in Microsoft Edge - use this to preview changes
- **No build step**: Static HTML file; changes take effect immediately upon browser refresh
- **Asset paths**: Images referenced with relative paths - keep them in root directory

## Important Conventions
- **ID naming**: Prefix element IDs with their type or purpose (e.g., `#main-content` not just `main`)
- **Language attribute**: Always maintain `lang="vi"` in `<html>` tag for Vietnamese content
- **Semantic HTML**: Use proper heading hierarchy (`h1` for title, `h2` for sections) and semantic elements (`<table>`, `<ol>`, `<ul>`)
- **External links**: Use `target="_blank" rel="noopener noreferrer"` for safety

## When Making Changes
1. Keep single-file structure (no external stylesheets currently)
2. Maintain Vietnamese language and Vietnamese content context
3. Test preview in Edge via launch configuration
4. Verify image asset references remain valid
5. Preserve centered, accessible layout design
