# Intent Definitions (Labeling Guidelines)

This doc defines how queries are labeled in `dataset.csv`.

## 1) Informational
User wants to learn or understand something.

**Common signals**
- “how to”, “what is”, “why”, “best way to”
- comparisons, explanations, guides

**Examples**
- how to clean a cast iron pan
- symptoms of vitamin d deficiency
- best ai tools for students

## 2) Navigational
User wants to reach a specific site, page, brand, or service.

**Common signals**
- brand/site names
- login pages, portals, specific destinations

**Examples**
- youtube studio login
- chase bank customer service
- reddit r/nba

## 3) Transactional
User wants to buy, download, subscribe, book, or complete an action.

**Common signals**
- “buy”, “deal”, “price”, “coupon”, “order”
- subscriptions, signups, downloads

**Examples**
- buy airpods pro 2
- netflix subscription cost
- download obs studio

## 4) Local
User wants something nearby or location-based.

**Common signals**
- “near me”, city names, “open now”
- restaurants, services, attractions

**Examples**
- coffee shop near me
- cheap dentist spokane
- hiking trails in seattle

## Tie-break rules
If a query could fit multiple intents:
1) Choose the intent that best matches the user's likely next action.
2) If the query includes a clear brand/page destination → Navigational.
3) If the query includes purchase/action language → Transactional.
4) If the query implies proximity/location need → Local.
5) Otherwise → Informational.
