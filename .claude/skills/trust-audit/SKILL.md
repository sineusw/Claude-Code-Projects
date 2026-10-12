---
name: trust-audit
description: Evidence-based privacy/trust audit for products handling user data, uploads, AI providers, subscriptions, or public marketing claims. Use before launch. Not legal advice.
disable-model-invocation: true
---

Build a table from the actual code and config (not from generic policy text): **issue | applies? | current implementation | missing work | verification | owner**.

Cover:
1. Data inventory: what is collected, why, where it goes, who can access, retention.
2. Processors: AI providers, analytics, crash reporting, storage, email, payments. Mark functional vs marketing/tracking; confirm users are told.
3. Representations match behavior: no invented testimonials, users, stats, or guarantees; structured-data ratings only if real.
4. Deletion: DB rows, uploaded originals, thumbnails/derivatives, caches, search indexes, provider copies; document backup retention honestly.
5. Storage privacy: user uploads private by default; public assets separated.
6. Billing: price, trial conversion, renewal timing and cancellation are clear; test cancellation in-app AND at the billing provider; reminders where applicable.
7. User safety handling only if the product has open-ended conversation or similar exposure.

Rules: don't claim legal compliance; flag items needing counsel and jurisdiction checks. Dollar penalty figures from social videos are unverified; do not use them. Don't write policies that promise things we haven't implemented.
