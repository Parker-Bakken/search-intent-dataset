# Rater Calibration Guide

This document simulates a basic calibration process used in search quality rating and data labeling projects.

Calibration ensures that different raters interpret queries and label intent consistently.

---

# Calibration Example 1

Query:
apple store

Possible interpretations:
1. User wants to visit the Apple Store website
2. User wants to buy Apple products
3. User wants a nearby Apple retail location

Chosen Label:
Navigational

Reasoning:
Most users searching "apple store" intend to reach Apple's official store page.

Tie-break rule:
Brand name + generic product destination typically indicates Navigational intent.

---

# Calibration Example 2

Query:
best buy laptop

Possible interpretations:
1. Researching laptops
2. Shopping for laptops at Best Buy

Chosen Label:
Transactional

Reasoning:
Brand + product combination often implies shopping intent.

---

# Calibration Example 3

Query:
weather seattle

Possible interpretations:
1. Local information request
2. General informational query

Chosen Label:
Informational

Reasoning:
Weather queries are typically categorized as informational even though they relate to a location.

---

# Calibration Example 4

Query:
cheap flights to paris

Possible interpretations:
1. Researching travel
2. Booking flights

Chosen Label:
Transactional

Reasoning:
The word "cheap" suggests purchase intent.

---

# Calibration Example 5

Query:
gym near me

Possible interpretations:
1. Looking for local gyms
2. Planning to sign up for membership

Chosen Label:
Local

Reasoning:
Queries containing "near me" are categorized as Local intent.

---

# Label Consistency Rules

When labeling ambiguous queries:

1. Identify the most likely next action of the user.
2. If a brand destination exists → Navigational.
3. If purchase/action language exists → Transactional.
4. If proximity/location is required → Local.
5. Otherwise → Informational.

---

# Why Calibration Matters

Calibration improves dataset quality by:

• reducing disagreement between raters  
• creating consistent training data  
• improving model reliability

This process mirrors the calibration sessions used in professional search evaluation teams.
