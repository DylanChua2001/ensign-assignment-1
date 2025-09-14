# Assumptions

During the implementation, some details in the provided design (`design.png`) were ambiguous. I made the following assumptions:

---

## 1. Fonts & Text
- The design font was unspecified. I assumed a **system font stack** (`Arial, sans-serif`) for simplicity, performance, and cross-platform consistency.  
- Text content in the cards is hardcoded placeholder text since no real data source was provided.

---

## 2. Icons & Images
- For the **Apple logo**, I used the FontAwesome Apple glyph with a CSS gradient (`background-clip: text`) to achieve the multi-coloured effect.  
- For other graphics (e.g., search icon, user avatar), I used **SVG** and **JPG** files because there was no one-to-one FontAwesome equivalent that matched the design.  
- Images such as `profile.jpg` are static placeholders; in a real application, they would come from user data or a CMS.  

---

## 3. Content & Dates
- Card titles, descriptions, and dates (e.g., “Two days ago”, “Last Tuesday”) are static placeholders derived from the design mockup.  
- No dynamic or interactive behavior was included, since the assignment specified HTML and CSS only.

---

## 4. Responsiveness
- I assumed the board should be **responsive**:  
  - 3 columns on desktop.  
  - 1 column on mobile (`max-width: 768px`).  

---

## 5. Accessibility
- Added `alt` text for images where appropriate.  
