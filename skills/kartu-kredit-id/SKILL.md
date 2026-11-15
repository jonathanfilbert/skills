---
name: kartu-kredit-id
description: |
  Research and compare Indonesian credit cards (kartu kredit Indonesia) for miles, points and cashback, using live web sources. Indonesia only: IDR, Indonesian issuers, local loyalty programs. Not for US or other markets.

  Trigger Scenarios:
  - User asks which kartu kredit to get in Indonesia (miles, KrisFlyer, GarudaMiles, Asia Miles, AirAsia, cashback)
  - User wants to compare two or more Indonesian cards, or check one card's earning rate, conversion ratio, exclusions, caps, annual fee or income requirement
  - User asks whether a card was or will be devalued (devaluasi), or what changed recently
  - User plans a large spend (wedding, renovation, tuition abroad, travel) and wants the card that earns the most on it
  - User asks to verify a claim, check whether a source is credible or up to date, or to monitor devaluations
  - User mentions PinterPoin, Cermati, Reward BCA, Yay Points, Voyage Miles, UNI$/UOB Points, Poin Xtra
---

# Kartu Kredit Indonesia

Indonesia-only credit card research. Answer in the user's language (Indonesian, English or mixed). Amounts in IDR.

## Rules

1. **Search first.** Terms change often. Never state an earning rate, ratio, fee, cap or exclusion from memory. If no source was found for a figure, write "belum terverifikasi".
2. **Collect from several sources, then check them** (see Source credibility). Never rely on one page.
3. **Cite every figure** with its source and date. Separate **confirmed** (issuer source) from **assumption**.
5. **Customer service has no reliable public data.** Do not infer it from affiliate articles or bank-wide awards. Say so, and tell the user to test the contact center before applying.
6. Do not give financial advice as certainty. Give the facts, a recommendation with its trade-offs, and what to verify.

## Workflow

1. **Get the profile** (ask at most one question, only if missing): monthly income, existing bank/payroll, expected monthly spend, preferred airlines, what matters most (flexibility, earning, ease, fee).
2. **Shortlist** 3-5 cards from current sources. Prefer cards that match the profile's income and bank relationship.
3. **Verify each card** against the checklist below, using the issuer page first.
4. **Run the devaluation watch** for each issuer (see below).
5. **Output** in the format below.

## Source credibility

Collect at least one issuer source plus two independent secondary sources per card, then grade them.

| Tier | Sources | Use for |
| --- | --- | --- |
| 1 | Issuer pages, T&C PDFs, announcements (`*.co.id`, `ocbc.id`, `jenius.com`, bank "pengumuman"/"informasi perubahan" pages); Bank Indonesia, OJK | Any figure. Final authority. |
| 2 | PinterPoin (`pinterpoin.com`), Bisnis, Kontan, Infobank, Detik Finance | Devaluation news, dated announcements, reviews. Verify the numbers against Tier 1. |
| 3 | Cermati, "best card" listicles, affiliate blogs (e.g. kiakrikil, industry.co.id) | Leads only. Often outdated, and may be written to earn referral fees. |

Checks before using a figure:

1. **Date.** Find the publish/update date and the effective date of the terms. Earning rates, ratios and fees older than 12 months are "possibly outdated" unless an issuer page confirms them.
2. **Conflicts.** If sources disagree (for example two different Rp-per-mile rates), the issuer page wins. State the conflict and both values.
3. **Bias.** Note when a source sells products tied to the topic (PinterPoin sells courses; affiliate sites earn per application). Use their facts, discount their rankings and "best card" verdicts.
4. **Independence.** Two pages that repeat the same table or text are one source.
5. **Mismatch between card tiers.** Check the exact card variant (e.g. PRVI Miles vs PRVI Miles Visa Infinite Privilege); figures differ by variant.

Give each card a confidence level: **High** (issuer source, current), **Medium** (reputable secondary, issuer source not reachable), **Low** (Tier 3 only or dated).

## Devaluation watch

Banks in Indonesia devalue often. For each issuer, check the last 24 months and anything announced but not yet effective.

1. Search PinterPoin's devaluation tags and `pinterpoin devaluasi <bank>`.
2. Search the issuer's announcement pages: `pengumuman perubahan ketentuan kartu kredit <bank>`, `informasi perubahan <card>`.
3. Search news for `<bank> kartu kredit perubahan poin <year>`.
4. Check the loyalty programs too, since award-chart devaluations cut the value of points (KrisFlyer, GarudaMiles, Asia Miles, AirAsia).

Count these as devaluations: higher IDR per point/mile, worse conversion ratio, new or lower earning caps, new exclusions, higher minimum or lower cap on redemption, higher annual fee or harder waiver, removed lounge/benefits, shorter points validity, and welcome bonuses raised "as compensation" for a cut.

Report per issuer:

- Dated list of changes (what, old value, new value, effective date, source)
- Pending changes with future effective dates
- Risk: **Low** (no change found in 24 months), **Medium** (one), **High** (two or more, or one in the last 6 months)

Never claim "no devaluation". Write "none found in the sources checked up to <date>". Tell the user to re-check right before applying, and offer to schedule a recurring check.

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
2. **Comparison**: one short line per card with earning, partners, annual fee, income requirement, last devaluation, devaluation risk, and source confidence.
3. **Fit to the user's criteria**: ✅ / ⚠️ / ❌ per criterion, one phrase each.
4. **Verify before applying**: unresolved items.
5. **Sources**: `[Title](URL)` with date.

Keep it short and copy-ready.
