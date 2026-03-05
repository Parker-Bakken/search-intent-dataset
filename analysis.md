# Dataset QA & Summary

## Quick QA checks
- Each row has: query, intent, notes
- Intents are limited to: Informational, Navigational, Transactional, Local
- Notes provide a short justification to support consistency

## Basic label distribution (manual estimate)
This dataset intentionally includes:
- a large Informational portion (most common in search)
- a balanced mix of Navigational and Transactional
- a solid Local section with "near me" and city-based queries

## Consistency examples
- Brand + login → Navigational (e.g., "gmail login")
- Buy/order/subscribe/download → Transactional (e.g., "download obs studio")
- Near me/city/service open now → Local (e.g., "dentist open now")
- Otherwise → Informational (e.g., "what is zero trust security")

## How to expand
To scale this dataset:
1) Add 20 queries per intent category (80 more total)
2) Add a "confidence" column (high/medium/low)
3) Add ambiguous queries and document tie-break reasoning
4) Add a second pass review to simulate real QA
