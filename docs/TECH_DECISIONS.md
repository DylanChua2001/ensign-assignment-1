# Technical Decisions

This document explains the reasoning behind the technical and architectural choices I made during the assignment.

---

## 1. Overall Approach
- Implemented the design in **HTML** and **CSS** as required.
- Avoided frameworks.

---

## 2. CSS Architecture
- **Structure**: Single `styles.css` with grouped sections (navbar, board, cards).

---

## 3. Layout & Responsiveness
- **Board**:  
  - Used **CSS Grid** with a fixed 3-column layout for desktop.  
  - On smaller screens (`max-width: 768px`), switched to a **flex column** layout so each column stacks vertically.  
- **Navbar**:  
  - On desktop, elements are arranged horizontally with logo, search bar, and user info.  
  - On small screens, the navbar switches to a **vertical stack**, with the search bar appearing above the user avatar and name.  

---

## 4. Accessibility
- Used semantic elements (`<header>`, `<h2>`, `<p>`, etc.).
- Added `alt` text for images (`profile.jpg`, icons).
- For the Apple logo, I used the FontAwesome glyph with a CSS gradient (`background-clip: text`) instead of an SVG/PNG. 
This approach is lightweight (no extra assets), scalable with `font-size`, and easy to update via CSS, while still achieving the required multi-coloured effect.
- For other icons and images where no one-to-one FontAwesome match existed, I used **SVG** (e.g., search icon) or **JPG** (e.g., profile avatar) as static assets. This ensured fidelity with the provided design while keeping the implementation lightweight.

---

## 5. Assets & Fonts
- Design font not specified → used **system font stack**.
- Images stored locally in `/src`; placeholders used where the design was vague.


---

## 6. Trade-offs & Known Limitations
- Fonts may not match pixel-perfect to design due to substitution.
- Hardcoded content; in production would fetch dynamically from API.

---
