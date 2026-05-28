# Detailed Project Steps

## Setup
Installed Tailwind, and created folders to contain index.html, start watcher, create git repository, source reference websites for design tips.

1. Mapped out website idea, theme colours and title
   - Title: Meubles & Co
   - Theme: Professional, Luxury
   - Colours: void `#080C10`, abyss `#0D1520`, midnight `#1B3A5C`, horizon `#4A7FA8`
   - Contents: Luxury furniture collections, showrooms, about us, home, contact

2. Started with this skeleton
3. Added meta information, link to output CSS folder and added title
4. Defined colours in input.css

## Navigation
5. Added a nav element and include the titles of other pages, created pages in src folder
6. Plan page layout:
   - Page 1: Home with hero section, captures attention
   - Page 2: Current seasonal collection (gallery)
   - Page 3: Showrooms
   - Page 4: About Us
   - Page 5: Contact

7. Added utility classes so nav bar appears central, has its own background colour and font matches the theme (`text-white hover:text-gold transition-colors duration-300 p-6`) — fading transition effect so it turns gold on hover
8. Add top bar — "Bespoke Furniture"

## Homepage and Hero Section
9. Add title using Cormorant Garamond sourced from Google Fonts
10. Add Est. 1925 date and italicise — added a custom utility class in `input.css` using `@layer utilities` as Tailwind v4 wasn't generating the italic utility automatically
11. Adjust margins on title and Est. 1925 so they appear closer together
12. Source imagery and create an images folder within src
13. Add hero imagery and text:
   - Changed from `img` tag to a `div` as background image to allow text overlay
   - Dark overlay added with fade effect via `bg-linear-to-t` — later extended from half to two thirds height
   - Wording added — "sustainably sourced, handcrafted..."
   - Button created linking directly to collection page with hover transition — letter spacing set to `-0.2em`
   - Fine-tuned design — shadow added to hero text, left-side gradient added for contrast, underline added to nav items via `border-b`

14. Footer developed with newsletter sign-up — "Join the Meubles & Co Circle"
    - Terms and conditions, privacy policy and rights reserved statement added
15. Header and footer replicated across all pages with nav correctly linked
16. Semantic elements included throughout — e.g. `<main>`, `<nav>`, `<footer>`

## Seasonal Collection
17. Source imagery for seasonal collection placed within a grid
18. Added a hero image labelled Navy Edit Autumn 2026 — dark overlay (`black/70`) positioned absolutely on relative parent. Text stacked vertically via flex column, centred via `items-center`, `justify-center` and `inset-0`
19. Separated imagery into bedroom and bathroom spaces with formatted section headings
20. Bedroom images — three side by side with no gaps using flex. Each image fitted to column width via `object-cover` without stretching
21. Philosophy text added — "Crafted from Earth" styled larger and brighter. Thin gold underline created via `bg-gold`, 1px height, centred via `mx-auto` with vertical spacing via `my-8`
22. Large Moroccan tile bathroom image added — text positioned via percentage values for `bottom` and `left`, max width set to 55%
23. Responsive text sizing applied — text appeared too large on smaller screens so `md:text-sm` used for medium screens and above
24. Additional bathroom imagery added in varied aspect ratios — `16/7` for wide image, `3/4` for five smaller images in a 5-column grid

## Showroom Listing
25. Hero image added with gradient applied to top and left, font styled with `tracking-widest`
26. Listings added for five upcoming locations — Kensington, Mayfair, Belgravia, Harrogate and Edinburgh
27. Hover effect applied — gold text brightens to `gold/60` and subtle white background appears via `hover:bg-white/5` over 300ms. `group` placed on parent row and `group-hover` on children so all children respond together

## About Us
28. Source royalty-free imagery — carpenter, close-up materials shots
29. Hero section created with heading "A Century of Craft"
30. Further sections added detailing brand mission and origin story
31. Large editorial quote inserted — `text-5xl`, `leading-snug`, centred via `mx-auto`
32. Gray `border-y` dividers added between sections using `white/10` opacity
33. Short gold underline decorators added via `<span>` with `bg-gold`
34. Closing full-width image added — text and overlay both absolutely positioned within a relative parent using `inset-0`

## Contact Page
35. Background set to `gold/10` to differentiate from main product pages
36. "We'd Love to Hear From You" heading absolutely positioned within a relative parent image — 300px tall, full screen width
37. Same font styling applied to headings — centred, shadow added for depth, gray overlay across image
38. Form centred via `mx-auto`, max width set via `max-w-2xl`
39. Form styled with `rounded-lg`, `shadow-md` and `bg-white` to stand out from gold background
40. Three fields created:
    - Name field
    - Email field
    - Message field with submit button
41. Spacing between fields via `mb-6`
42. Label tags styled with `text-gray-700`, `font-medium`, `text-sm`
43. Input types set — `type="text"` for name, `type="email"` for email. `id` matches `for` value on each label
44. Input styling — full width, padding, gold border, gold focus ring via `focus:outline-none focus:ring-2 focus:ring-gold`
45. Same styling applied to email and message fields
46. Submit button inverts to navy on hover via smooth transition duration

## Final Steps
47. Complete README and push to GitHub