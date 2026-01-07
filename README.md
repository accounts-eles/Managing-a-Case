📂 Managing a Case: Interactive Case Study Template

A structured, professional-grade template designed for evaluating ethical dilemmas, clinical scenarios, or administrative processes. This interface uses a combination of high-level guidance and granular, accordion-based scenario analysis.

🚀 Live Demo

Explore the Managing a Case Interface Here

✨ Project Overview

The "Managing a Case" template provides a robust framework for comparative learning. It is specifically designed to show the contrast between "Poor Practice" (Risks) and "Best Practice" (Solutions) within specific scenarios.

Key Features

Guidance Protocol Section: A persistent, light-teal anchor box (#d2f0f0) that outlines the general principles or steps required to resolve any case within the module.

Dynamic Accordion System: Interactive headers that utilize a "one-at-a-time" expansion logic. Opening a new scenario automatically collapses previous ones to maintain user focus.

Dual-Panel Comparison: Each scenario features a side-by-side (or stacked on mobile) grid comparing:

🔴 Poor Practice: Highlighted with a red border (border-red-500) and exclamation icons to signal risks or common errors.

🟢 Best Practice: Highlighted with a green border (border-green-500) and checkmark icons to indicate the gold standard or ethical path.

Smooth Transitions: JavaScript-calculated scrollHeight ensures that accordion expansions are fluid regardless of the amount of text content.

🎨 Visual Identity & UI Standards

The interface adheres to a sophisticated professional palette:

Primary Navy (#1f2a52): Used for authoritative headers and guidance text.

Bright Teal (#00bec7): Powers the accordion headers to draw immediate visual attention to the interactive elements.

Semantic Accents: Red and Green are used strictly for instructional feedback (Warning vs. Success).

Typography: The Inter font family is utilized for high legibility across varying text densities.

🛠️ Technical implementation

Accordion Logic

The expansion is handled via a specialized JavaScript function toggleAccordion(button).

It toggles the .active class on the parent item.

It dynamically adjusts max-height from null to scrollHeight + "px" to enable CSS transitions on elements with unknown heights.

It manages corner rounding (rounded-xl vs rounded-t-xl) to ensure the header stays visually connected to its content when open.

Responsive Design

Grid System: Uses Tailwind's grid-cols-1 lg:grid-cols-2 to ensure the risk/practice panels stack vertically on mobile devices but sit side-by-side on desktops.

Iconography: SVG icons from the Heroicons set are used for "Lock", "Clipboard", and "Documentation" motifs to provide visual context for each scenario.

📂 Project Structure

Case_Management_Activity/
├── index.html          # Main application file (HTML/CSS/JS)
├── README.md           # Project documentation
└── .github/workflows/  # Automated deployment and preview scripts


📖 Customization Guide

Adding New Scenarios

To add a scenario, duplicate an .accordion-item div. Each scenario follows this inner structure:

Header Button: Contains the icon and the Scenario Title.

Dilemma Paragraph: Summarizes the conflict.

Grid Container: Contains the two card-panel divs for Poor vs. Best Practice.

Color Customization

Update the CSS classes .bg-brand-accent-bright or .bg-brand-light-accent in the <style> block to align the interface with different department branding.

📄 License

MIT License - Created for the accounts-eles instructional design ecosystem.
