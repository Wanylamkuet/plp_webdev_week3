# SpendWise — Budget Tracker (Visual Design Challenge)

## Overview
**SpendWise** is a Budget Tracker web application styled for the **Design the Visual Identity of Your Budget Tracker** assignment in [Web Development Fundamentals](https://academy.powerlearnprojectafrica.org/module/6a7d55799bdd17521a677e8a?study=false). Building upon the structure and selectors from earlier weeks without adding new HTML markup or functionality, this update focuses on visual hierarchy, color consistency, typography, form/table polish, and the CSS Box Model.

## Project Structure
- `index.html` — The existing Budget Tracker markup (`header`, `#add-expense-section`, `#expenses-list-section`, form controls, and expense table).
- `style.css` — Combined and refined stylesheet implementing the visual identity, custom fonts, box model card layout, and interactive states.
- `README.md` — Project documentation explaining the design choices and how each stylesheet section works.

## Visual Design & CSS Breakdown

### 1. Color Palette (`:root` Custom Properties)
A consistent finance-inspired palette is defined using CSS variables in `style.css` and applied across the interface:
- **Page Background (`--bg-page`: `#f1f5f9`)**: Soft cool slate background that reduces eye strain and makes white cards stand out.
- **Card Surface (`--bg-card`: `#ffffff`) & Subtle Tint (`--bg-subtle`: `#f8fafc`)**: Used for card containers, zebra-striped table rows, and `<details>` blocks.
- **Primary (`--color-primary`: `#1e3a5f`)**: Deep navy used for main/section headings, the page header card, and the table header row.
- **Accent (`--color-accent`: `#2563eb` / hover `#1d4ed8`)**: Royal blue applied to action buttons, focus rings, and the top accent border of the Add Expense card.
- **Secondary (`--color-secondary`: `#0d9488`)**: Teal accent on the top border of the Expenses List card to visually distinguish the two main sections.

### 2. Typography ([Google Fonts](https://fonts.google.com))
- **Headings & Buttons (`Poppins`)**: Applied to `h1`, `h2`, `h3`, `summary`, table headers, and buttons to establish clear hierarchy and visual emphasis.
- **Body, Forms & Table Content (`Inter`)**: Applied across `body`, labels, inputs, selects, and table cells for clean legibility and consistent alignment.

### 3. Expense Table & Add Expense Form Styling
- **Box-Sizing & Spacing**: `box-sizing: border-box` prevents inputs (`width: 100%`) and tables from overflowing their parent containers, paired with comfortable cell and input padding.
- **Form Controls**: Styled `.form-group` labels, `input:not([type="submit"])`, `select`, and `textarea` with rounded corners (`border-radius: 8px`), subtle borders, and `:focus` highlight rings.
- **Table Structure**: Styled `table` with `border-collapse: collapse`, a high-contrast `thead tr` header row, alternating `tbody tr:nth-child(even)` rows, and a smooth `tbody tr:hover` state.

### 4. CSS Box Model & Visual Cards
Each major section is styled as a distinct card using `margin`, `padding`, `border`, and `border-radius`:
- **Page Heading Card (`header`)**: Deep navy card with generous padding, rounded corners (`12px`), and bottom margin separating it from the form.
- **Add Expense Form Card (`#add-expense-section`)**: White card with `24px` padding, `1px` border with a `4px` royal blue top accent, `12px` border-radius, and bottom margin.
- **Expense Table Card (`#expenses-list-section`)**: White card with `24px` padding, `1px` border with a `4px` teal top accent, `12px` border-radius, and clean spacing around the table.

## How to Run Locally
1. Clone or download the repository containing `index.html`, `style.css`, and `README.md`.
2. Open `index.html` in any web browser.