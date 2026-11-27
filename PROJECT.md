# Project Context

## Repository
https://github.com/Jimz364/FoodWisePH.git

## Deployment
Not deployed yet.

## Product
Bantay Kusina — a household food waste prevention simulator.

## Audience
Primarily Filipino households and students living alone who need help managing the food they already have.

## Goal
Help users reduce avoidable food waste by tracking household food, estimating spoilage risk, recommending what to consume first, and comparing how household choices affect estimated waste over time.

## Brand
Bantay Kusina. Filipino-inspired, approachable, practical, and sustainability-minded. Working tagline: "Bantay sa pagkain, bawas sa sayang."

## Visual Direction
Not decided yet. Await the user's design reference before defining the visual system.

## Page Structure
To be finalized after the design reference. The app should provide a welcoming start point, household dashboard, inventory management, Smart Pantry Scan, simulation scenarios, results/analytics, and a food storage guide.

## Copy Direction
Use clear, friendly English with familiar Philippine household examples and metric units. Avoid overly technical wording. Explain that shelf-life and spoilage outputs are estimates, not food-safety guarantees.

## Assets
No user-provided brand or food assets yet. Smart Pantry Scan is planned as single-photo scanning for multiple groceries. Recognition should be treated as suggestions that users review and confirm; unsupported foods can be added through the catalog or manually.

## Functionality
Planned features:
- Preloaded sample household inventory and custom food entries.
- Food catalog with Filipino household staples across meat/poultry, seafood, vegetables, fruits, dairy/eggs, grains/rice, and cooked meals/leftovers.
- Food records include food type, purchase date, storage method, quantity/unit, suggested shelf life, and optional purchase price in PHP; users can edit suggested values.
- Estimated shelf life varies by food type and storage method, with a clear explanation of each item's risk status.
- Risk labels: Fresh, Use Soon, Consume First, and Past Estimated Shelf Life.
- Single-photo Smart Pantry Scan for multiple foods, with review/correction before batch adding. Prefer browser-based recognition where practical; maintain a replaceable recognition layer and catalog/manual fallback for unsupported items.
- Household size affects estimated consumption.
- Scenario simulator compares three matching starting inventories: Responsible Household (follows recommendations), Neglectful Household (delays consumption by two days and ignores priority recommendations), and Improved Storage (applies suggested storage methods, with manual adjustments).
- Simulation duration choices: 7, 14, or 30 days; support both day-by-day and full-run modes.
- Analytics compare estimated waste, saved quantity, spoiled item count/quantity, waste percentage, and optional estimated monetary loss in PHP.
- Food storage education guide.
- Browser-local inventory persistence, JSON export/import, and reset.
- Accessible, responsive interface with simple navigation.

## Avoid
Don't use food-risk estimates as definitive safety advice. Don't infer unknown purchase dates, quantities, or storage states from photos. Avoid forcing users to enter items one by one when batch scan or catalog selection can help. Avoid clutter, unnecessary animation, technical jargon, and unsupported claims about image recognition accuracy. Keep the implementation lightweight and self-contained unless a real technical requirement justifies otherwise.

## Current Decisions
The user approved all recommended product and simulation decisions, including Smart Pantry Scan (one photo for multiple items), review-before-import, temporary photo handling with confirmed food information retained, explanations for risk rankings, an educational storage guide, sample/custom inventory, editable shelf-life suggestions, scenario comparison, 7/14/30-day simulations with step/run controls, household-size-based consumption, PHP loss estimates, dashboard/filtering, and local save plus JSON import/export. Product name is **Bantay Kusina**. Visual reference has not yet been supplied.
