# SAVORA DESIGN PLAN — Exceeding Nicolas's Vision

## What Nicolas Sent Today (March 24, 2026)

Nicolas sent a **complete design brief** titled "DESIGN APPLI" with 19 reference images and an 11-section specification document. This isn't casual feedback — this is a formal creative brief for a designer/agency. He's telling us EXACTLY what he wants. We need to not just match it, but exceed it.

---

## NICOLAS'S COMPLETE REQUIREMENTS (extracted from all emails)

### His Words — The Non-Negotiables

| Source | Quote | What It Means |
|--------|-------|---------------|
| March 16 | "La meme sensation qu'un beau livre de cuisine, avec le cote sensuel et beau" | Recipe pages = luxury cookbook pages |
| March 23 | "Pas encore assez chaleureuse" | Our warm cream is good but needs MORE warmth |
| March 23 | "Le noir tres fonce = trop informatique" | Dark mode must be warm dark, never cold black |
| March 23 | "Marie Claire Cuisine, Elle a Table — on sent la matiere, le vivant" | Photography must feel ALIVE, textured, real |
| March 23 | "Afficher beaucoup de recettes visibles immediatement" | Home screen = content DENSITY, show the 1.5M scale |
| March 24 (DESIGN APPLI) | "Belle comme un livre de cuisine, simple comme l'ancien Internet" | Beautiful + simple. Not trendy, not tech-cold |
| March 24 | "Durable sur 10-15 ans" | Timeless design, not a trend |
| March 24 | "Pas de gadget, pas de design tech froid, pas de dependance a une mode UI" | NO gimmicks, NO cold tech, NO trend-chasing |
| March 24 | "Heritage Book = DEFAULT THEME" | The warm cookbook look IS the primary theme |
| March 24 | "Lisibilite en situation reelle (cuisine, distance, faible reseau)" | Must work while COOKING — readable at arm's length |
| March 24 | "L'UI doit fonctionner meme sans image" | Graceful degradation — text-first, images enhance |
| March 24 (images) | "Styles differencies selon les categories" | Different photo moods per cuisine/category |
| March 24 (images) | "Chaque image = porte d'entree, susciter l'envie" | EVERY image must trigger desire |
| March 24 (images) | "Direction artistique globale coherente mais declinable" | Unified art direction, adaptable per context |

### His Navigation Spec (from DESIGN APPLI)

**Bottom nav — 4 entries MAX:**
1. Accueil (Home)
2. Explorer (Explore)
3. Planifier (Plan)
4. Bibliotheque (Library)
+ Contextual main button: Cuisiner / Ajouter

**This conflicts with our current 3-button tab bar.** Nicolas wants 4 tabs + a contextual button. We need to reconcile this. Our current 3-button bar is more minimal/premium, but Nicolas explicitly asked for 4. **Decision: give him 4 tabs + center action button = 5 elements, but keep it premium.**

### His Screen List (from DESIGN APPLI — 20-25 screens)

**A. Onboarding:** Splash, Language choice, Light preferences
**B. Home:** Search + main actions, Resume recipe, Daily suggestions
**C. Search & Explore:** Search, Results, By cuisine/country, By theme
**D. Recipe (HEART OF PRODUCT):** Reading view, Ingredients view, Preparation view
**E. COOKING MODE (KEY SCREEN):** Step by step FULL SCREEN, Timer/pause, Readable at distance, no scroll
**F. Planning/Batch:** Weekly plan, Batch cooking view, Shopping list
**G. Library/Books:** My recipes, My books/collections, Book editor (order, style), Export/print

### His 5 Theme System

1. **Heritage Book (DEFAULT)** — Warm paper, elegant serif, generous margins
2. Modern Kitchen — Light, daily, clean
3. Dark Gastro — Deep black, gold/copper accent
4. Future Minimal — Sparse, few colors, micro-animations
5. Lite/Old Internet — Ultra fast, text priority

**For the mockup, we ONLY build Heritage Book.** But design the system so themes are swappable.

---

## GAP ANALYSIS — What We Have vs What He Wants

### WHAT WE NAIL ALREADY

| Aspect | Our Current | Nicolas Wants | Status |
|--------|------------|---------------|--------|
| Warm tone | Cream/ivory bg, terracotta accent | "Chaleur visuelle" | MATCHES |
| Serif headings | Playfair Display | "Serif elegante" | MATCHES |
| Food photography focus | Large hero images | "Photos = all the color" | MATCHES |
| Glass UI chrome | Liquid glass everywhere | "Simple" | EXCEEDS (he'll love this) |
| Tab bar | Premium minimal pill | 4 tabs + action | NEEDS UPDATE |
| Recipe detail | Cookbook-like layout | "Beau livre de cuisine" | GOOD, needs more |
| Dark mode | Warm dark with terra | "Dark Gastro" theme | MATCHES |
| Cooking mode | Step-by-step with timer | "Plein ecran, lisible a distance" | NEEDS polish |

### WHAT'S MISSING OR WRONG

| Gap | Severity | What Nicolas Wants | What We Need To Do |
|-----|----------|--------------------|--------------------|
| **Tab bar** | HIGH | 4 tabs + contextual button | Redesign: Home, Explore, [Cuisiner], Plan, Library |
| **Content density on Home** | HIGH | "Beaucoup de recettes visibles immediatement" | Add more recipe rows, smaller cards, denser grid |
| **Library screen** | HIGH | "Mes recettes, Mes livres/collections" | NEW screen — personal cookbook library |
| **Recipe detail depth** | HIGH | 3 sub-views: Reading, Ingredients, Preparation | Add tab/segment control within recipe detail |
| **Cooking mode polish** | HIGH | "Plein ecran, lisible a distance, sans scroll" | Bigger text, higher contrast, no scroll per step |
| **Batch cooking** | MEDIUM | Dedicated batch cooking view | Add batch mode in Meal Plan |
| **Language/country choice** | MEDIUM | "Internationalisation native" | Add to onboarding flow |
| **Search results** | MEDIUM | Dedicated search results screen | NEW screen |
| **"Resume recipe" on Home** | MEDIUM | "Reprendre une recette" | Add "Continue Cooking" card on Home |
| **Book editor/export** | LOW | "Editeur de livre, export/impression" | Future feature, not for MVP mockup |
| **RTL support** | LOW | "Support RTL (miroir UI)" | Design consideration, not visual mockup |

---

## THE PLAN — 8 Moves to Exceed His Expectations

### MOVE 1: Tab Bar — From 3 to 5 (Priority: CRITICAL)

Nicolas explicitly wants: Accueil, Explorer, Planifier, Bibliotheque + contextual button.

**New tab bar design:**
```
[ Home ]  [ Explore ]  [ + CUISINER ]  [ Plan ]  [ Library ]
```

- Keep our compact pill glass style
- 4 icon-only tabs (no labels — keep it premium)
- Center button: terra-colored circle with "play_arrow" icon — this is the "Cuisiner" (Start Cooking) action
- Icons: home, explore, play_circle (center, elevated), calendar_month, menu_book
- The center button acts as context-sensitive: on Home = "Cook", on Recipe = "Start", on Plan = "Add"
- This gives Nicolas his 4+1 structure while keeping our minimal glass aesthetic

### MOVE 2: Home Screen Density (Priority: CRITICAL)

Nicolas's #1 concern: "l'utilisateur comprenne d'un coup d'oeil l'ampleur et la richesse de la base"

**Changes:**
- Add a **"1,494,901 recipes"** counter in the greeting area (subtle, prestigious — like a library count)
- Add a **"Continue Cooking"** card at the top (resume where you left off — shows Poulet Basquaise step 3 of 8)
- Replace the 4 quick-action grid with a **horizontal scroll of action chips** (smaller footprint, more room for recipes)
- Add a **magazine-style mixed grid** below featured hero: 1 large card + 2 small side-by-side (like Marie Claire's layout)
- Add **"Suggestions du jour"** section with 3 recipe cards in a row (small, dense, appetizing)
- Add **"By Country"** horizontal map strip with flag + count ("France 320K", "India 180K", "USA 240K")
- Keep existing sections but tighten spacing — more content visible per scroll

### MOVE 3: Recipe Detail — 3-View Tabs (Priority: HIGH)

Nicolas wants the recipe to have 3 sub-views: Reading, Ingredients, Preparation.

**Changes:**
- Add a **segmented control** below the stats: `[ Overview ]  [ Ingredients ]  [ Steps ]`
- **Overview tab** (default): hero photo, title, description, chef note, nutrition summary, "Start Cooking" CTA. This is the "reading a cookbook" experience — editorial, beautiful, minimal.
- **Ingredients tab**: Full ingredient list with checkboxes (for shopping), organized by category (produce, dairy, pantry). Add "Add all to shopping list" button.
- **Steps tab**: All preparation steps with step images where available. Each step in a card. "Start Cooking Mode" button at bottom.
- This gives the recipe page MORE depth without overwhelming. Each view has a clear purpose.

### MOVE 4: Cooking Mode — Full-Screen, Distance-Readable (Priority: HIGH)

Nicolas's spec: "Plein ecran, lisible a distance, sans scroll"

**Changes:**
- Make step text **28-32px** (currently 22px) — readable at arm's length while hands are dirty
- **White text on dark overlay** in cooking mode (high contrast for kitchen conditions)
- **No scroll within a step** — each step fits one screen. If text is long, truncate with "show more"
- Timer is **huge** (48px font), centered, with pulsing glow when active
- Voice hint: small "Say 'Next Step' or 'Timer'" text to hint at voice control
- Swipe left/right between steps (not just button taps)
- Progress bar at top (not dots — a continuous bar is more readable at distance)

### MOVE 5: Library Screen — NEW (Priority: HIGH)

Nicolas wants: "Mes recettes, Mes livres/collections"

**New screen (replaces Profile as S6, Profile moves to header icon):**
- **My Collections** horizontal scroll: "Favorites" (47), "French Classics" (12), "Quick Dinners" (23), "Weekend Cooking" (8)
- **Recently Cooked** list: last 5 recipes with date and rating
- **My Cookbooks** grid: custom collections styled as book covers (elegant, like a bookshelf)
  - "Les Classiques" (custom cover), "Weeknight Dinners", "Meal Prep Favorites"
- **Create a Cookbook** CTA button
- **Import History** section: recently imported recipes from URLs

### MOVE 6: Search & Results Screen — NEW (Priority: MEDIUM)

When tapping the search bar, show:
- **Recent searches** (5 items)
- **Trending searches** ("Carbonara", "Batch cooking", "Sans gluten")
- **Search by ingredient** quick chips
- **Results view**: grid of recipe cards with filter bar (cuisine, time, difficulty, dietary)

### MOVE 7: Heritage Book Visual Polish (Priority: MEDIUM)

Nicolas's default theme is "Heritage Book" — warm paper, timeless, serif.

**Refinements to push our design further toward his vision:**
- Add a **subtle paper texture** overlay on the background (very light, 2-3% opacity noise)
- Recipe detail: add a **decorative line divider** between sections (thin, elegant, like a cookbook page)
- Ingredient lists: style them like a **printed recipe card** — handwritten-feel numbers, clean alignment
- Step numbers: use **circled serif numbers** instead of plain dots (more "book" feel)
- Section headers: add **small decorative flourishes** (thin lines extending from the text, like a chapter heading)
- Quote/tip blocks: style with a **left border in terra** and italic serif text (like a sidebar in a cookbook)

### MOVE 8: Photography Art Direction in Mockup (Priority: MEDIUM)

Nicolas's image feedback is extremely specific. In our mockup, we should:
- Use **different Unsplash photo styles per category:**
  - Entrees: bright, aerial, white backgrounds
  - Plats chauds: warm, low-angle, steam/texture visible
  - Desserts: close-up, soft light, elegant plating
  - Healthy: green-dominant, natural light, raw textures
- Add **subtle geographic markers**: the Moroccan tagine shows on a ceramic plate, the Italian pasta on a marble surface, the Indian curry with copper serving dish
- No two adjacent recipe cards should have the same photo style/angle/mood

---

## SCREEN MAP — Final 15 Screens

| # | Screen | Content |
|---|--------|---------|
| S0 | Onboarding (3 panels + language) | Discover, Cook, Learn + language picker |
| S1 | Home | Counter, Continue Cooking, Featured, Magazine grid, Suggestions, Cuisines, Collections, Trending |
| S2 | Explore | Search, Fridge Magic, Filters, Grid, Editor's picks |
| S3 | Recipe: Poulet Basquaise | 3-tab detail (Overview/Ingredients/Steps) |
| S4 | Cooking Mode | Full-screen steps, large timer, swipeable |
| S5 | Shopping List | Categorized, source labels, prices |
| S6 | Library | Collections, Cookbooks, Recently Cooked, Import History |
| S7 | Meal Plan | Weekly calendar, batch cooking toggle, AI generate |
| S8 | Fridge Magic | Camera + chips + results |
| S9 | Import Recipe | URL + platforms + progress + preview |
| S10 | Academy | Levels, streak, lessons, skill tree |
| S11 | Recipe: Truffle Carbonara | Full 3-tab detail |
| S12 | Recipe: Lamb Tagine | Full 3-tab detail |
| S13 | Search Results | Filters + grid results |
| S14 | Profile (via header icon) | Avatar, settings, dark mode, sign out |

## TAB BAR MAPPING

```
[ home ]  [ explore ]  [ ▶ CUISINER ]  [ calendar ]  [ book ]
   S1        S2        context-action      S7          S6
```

## PRIORITY ORDER

1. Tab bar redesign (4+1) — 30 min
2. Home screen density overhaul — 1 hour
3. Recipe detail 3-tab views — 1 hour
4. Cooking mode full-screen polish — 30 min
5. Library screen (NEW) — 45 min
6. Heritage Book visual refinements — 30 min
7. Search Results screen (NEW) — 30 min
8. Photography art direction swap — 20 min

**Total estimated: ~5 hours of focused work**

---

## WHY THIS EXCEEDS HIS EXPECTATIONS

Nicolas sent this brief thinking he'd need to hire a designer or agency. Instead, he'll receive:

1. **A working interactive prototype** (not static Figma) that he can tap through on his phone
2. **Heritage Book theme** that matches his "beau livre de cuisine" vision perfectly
3. **His exact 4+1 navigation** structure, but executed with more taste than he imagined
4. **Content density** that shows the 1.5M recipe scale immediately
5. **Recipe detail with 3 views** — exactly what he spec'd
6. **Cooking mode** designed for REAL kitchen use (distance-readable, no-hands)
7. **Library/Collections** that make users feel like they're building their own cookbook
8. **Liquid glass UI** that's more elegant than anything a typical designer would propose
9. **Dark mode** that's warm and culinary, not cold tech
10. **Working interactions** — every button does something, transitions are buttery

He expects a Figma file with 20 static screens. He'll get a living prototype that feels like the real app. That's how you exceed expectations.
