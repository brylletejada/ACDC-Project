# ACDC Pathways prototype

This is a no-build web prototype for the ACDC student opportunity hub. It is intentionally made with plain HTML, CSS, and JavaScript so the team can open it in Visual Studio Code or IntelliJ IDEA without setting up a framework first.

## Run it

1. Open the project folder in VS Code or IntelliJ IDEA.
2. Open `index.html` in a browser, or use a simple local server:

```bash
python3 -m http.server 8000
```

3. Visit `http://localhost:8000`.

## Current prototype features

- ACDC-inspired purple, pink, coral, and yellow visual system.
- Responsive desktop and mobile layout.
- Main navigation for Explore, Learning resources, Opportunities, and Student support.
- Search across pathways, resources, and opportunities.
- Detail modal for pathway, resource, and opportunity cards.
- Save/bookmark behavior stored in browser local storage.
- Progress card showing a student career-map journey.

## Suggested next implementation step

Replace the arrays at the top of `app.js` with API/database data. A simple first version of the database can use five core tables: `users`, `pathways`, `resources`, `opportunities`, and `saved_items`. The `pathways` table can connect to many resources and opportunities through join tables such as `pathway_resources` and `pathway_opportunities`.

The ACDC content used as inspiration includes Technology, Business, and Psychology learning pathways, a Browse → Sign Up → Learn → Earn journey, weekly discussion support, and volunteer opportunities. Confirm final copy and links with ACDC before treating the prototype content as production information.
