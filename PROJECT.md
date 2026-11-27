# Project Context

## Repository
https://github.com/Jimz364/FoodWisePH.git

## Deployment
Not deployed yet. Keep the project compatible with static hosting.

## Product
**BantayKusina** — Smart Household Food Waste Prevention Simulator.

## Audience
Primarily Filipino households and students living alone who need help managing the food they already have.

## Goal
Help users reduce avoidable food waste by tracking household food, estimating spoilage risk, recommending what to consume first, and comparing how household choices affect estimated waste over time.

## Brand
BantayKusina. Tagline: "Bantay sa pagkain, bawas sa sayang." Filipino, modern, approachable, practical, and sustainability-minded.

## Visual Direction
Dark mode by default with a user-controlled light/dark toggle. Use deep charcoal and muted forest-green surfaces, sage/lime accents, warm cream text, restrained amber/red freshness states, clear typography, rounded but restrained surfaces, and responsive layouts. The product should feel like a polished household utility. Avoid pure-black backgrounds, excessive glow, decorative gradients, clutter, and unnecessary animation.

## Page Structure
Single-page app with Overview, My Kusina inventory, Smart Pantry Scan, Simulation Lab, and Storage Guide. The overview highlights food needing attention and a quick pantry summary.

## Copy Direction
Use clear, friendly English with familiar Philippine household examples and metric units. Avoid overly technical wording. Explain that shelf-life and spoilage outputs are estimates, not food-safety guarantees.

## Assets
No user-provided brand or food assets. Smart Pantry Scan accepts one photo containing multiple items. Initial browser recognition uses COCO-SSD for a limited set of common visible objects (mapped to supported produce); users must review suggestions. Unsupported foods require manual entry. Photos are used temporarily for recognition and are not stored in pantry data.

## Functionality
- Preloaded sample household inventory and custom food entries.
- Food catalog with Filipino household staples across meat/poultry, seafood, vegetables, fruits, dairy/eggs, grains/rice, and cooked meals/leftovers.
- Food records include food type, purchase/prepared date, storage method, quantity/unit, editable suggested shelf life, and optional purchase price in PHP.
- Risk labels: Fresh, Use Soon, Consume First, and Past Estimated Shelf Life, with a short reason.
- Single-photo Smart Pantry Scan for multiple foods, with review and selection before adding. Recognition is limited and browser-based; manual entry is the fallback.
- Household size and 7/14/30-day duration controls for the scenario simulator.
- Compare Responsible Household, Neglectful Household (two-day delay), and Improved Storage scenarios.
- Show estimated waste, food used, and optional estimated value lost in PHP.
- Food storage education guide.
- Browser-local inventory persistence, JSON export/import, and reset capability.
- Responsive interface, accessible labels/focus states, and theme toggle.

## Avoid
Don't present estimated shelf life as a food-safety guarantee. Don't infer unknown purchase dates, quantities, or storage states from photos. Don't claim comprehensive image recognition. Avoid clutter, unnecessary animation, technical jargon, and unsupported claims. Keep implementation lightweight and self-contained.

## Current Decisions
The user approved the BantayKusina brand, dark-first design, and a light/dark theme toggle. Product decisions include sample/custom inventory, editable shelf-life suggestions, review-before-import photo scan, manual fallback, storage guide, household-size-based scenario comparison, 7/14/30-day durations, PHP value estimates, local persistence, and JSON import/export. Current implementation is a first working prototype in one self-contained `index.html`; the simulator is an educational simplified model and needs validation/refinement before making stronger claims.
