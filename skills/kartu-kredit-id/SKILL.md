---
name: kartu-kredit-id
description: |
  Research and compare Indonesian credit cards (kartu kredit Indonesia) for miles, points and cashback, using live web sources. Indonesia only: IDR, Indonesian issuers, local loyalty programs. Not for US or other markets.

  Trigger Scenarios:
  - User asks which kartu kredit to get in Indonesia (miles, KrisFlyer, GarudaMiles, Asia Miles, AirAsia, cashback)
  - User wants to compare two or more Indonesian cards, or check one card's earning rate, conversion ratio, exclusions, caps, annual fee or income requirement
  - User asks whether a card was or will be devalued (devaluasi), or what changed recently
  - User plans a large spend (wedding, renovation, tuition abroad, travel) and wants the card that earns the most on it
  - User mentions PinterPoin, Cermati, Reward BCA, Yay Points, Voyage Miles, UNI$/UOB Points, Poin Xtra
---

# Kartu Kredit Indonesia

Indonesia-only credit card research. Answer in the user's language (Indonesian, English or mixed). Amounts in IDR.

## Rules

1. **Search first.** Terms change often. Never state an earning rate, ratio, fee, cap or exclusion from memory. If no source was found for a figure, write "belum terverifikasi".
2. **Source priority:** (1) issuer's official page, T&C PDF or announcement (`*.co.id`, `ocbc.id`, `jenius.com`); (2) Bank Indonesia / OJK; (3) PinterPoin (`pinterpoin.com`) for devaluation news and reviews; (4) Cermati, Bisnis, Kontan, Infobank; (5) other blogs, only for opinion.
3. **Aggregator pages (Cermati, "best card" lists) lag.** If one conflicts with an issuer page, trust the issuer and flag the conflict.
4. **Cite every figure** with its source and date. Separate **confirmed** (issuer source) from **assumption**.
5. **Customer service has no reliable public data.** Do not infer it from affiliate articles or bank-wide awards. Say so, and tell the user to test the contact center before applying.
6. Do not give financial advice as certainty. Give the facts, a recommendation with its trade-offs, and what to verify.

## Workflow

1. **Get the profile** (ask at most one question, only if missing): monthly income, existing bank/payroll, expected monthly spend, preferred airlines, what matters most (flexibility, earning, ease, fee).
2. **Shortlist** 3-5 cards from current sources. Prefer cards that match the profile's income and bank relationship.
3. **Verify each card** against the checklist below, using the issuer page first.
4. **Check devaluation history** for each issuer: search `pinterpoin devaluasi <bank>` and the issuer's announcement page for the last 24 months.
5. **Output** in the format below.

## Per-card checklist

- Earning: IDR per 1 point/mile, domestic vs overseas, bonus categories
- Currency and conversion: points to each airline (KrisFlyer, GarudaMiles, Asia Miles, AirAsia, LinkMiles), ratios, minimum, monthly redemption cap, fee, instant vs manual
- Earning cap per billing cycle (some issuers tie it to credit limit)
- Excluded transactions: installments (cicilan), bill payment, tax, government, education, fuel, e-money top-up, insurance, digital ads
- Name-match rule: airline account name must equal cardholder name
- Points expiry
- Annual fee, waiver condition, supplementary card
- Minimum income, minimum/typical limit, application channel (app, web, branch)
- Welcome bonus: spend condition, time window, deadline
- Devaluation history with dates (earning, conversion, caps, exclusions, fees)

## Large one-off spend (wedding, etc.)

Also check: whether the merchant category earns points, whether the vendor adds a card surcharge (often larger than the points), per-transaction limit, temporary limit increase (TLI), whether installments earn, and whether the welcome-bonus window lines up with when payments actually start.

## Output format

1. **Pick** (1-2 lines): the card and the single biggest reason.
2. **Comparison**: one short line per card with earning, partners, annual fee, income requirement, last devaluation.
3. **Fit to the user's criteria**: ✅ / ⚠️ / ❌ per criterion, one phrase each.
4. **Verify before applying**: unresolved items.
5. **Sources**: `[Title](URL)` with date.

Keep it short and copy-ready.
