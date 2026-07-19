# Compliance policy

> **Status: not operational.** LeadFi requested read-only Reddit Data API access for the
> research described in the README; **access was not granted.** Nothing in this policy is
> currently running. This document records the read-only design and the rules that design
> commits to. It is a statement of intended behavior, not a description of a live system.
> No Reddit data is being accessed or stored.

The rules below would govern the tool only if access were ever granted under an appropriate
agreement with Reddit. This file is the single source of truth for the Reddit lane; any code
or configuration must derive from it, and divergence blocks merge.

## Read-only

1. Read endpoints only. It never posts, comments, votes, messages, edits, or deletes anything
   on Reddit.
2. No write access on the credentials, and none would be added under this app.
3. Not a participant. No automated replies, no interaction with users.

## Access

4. Access would be through the **official Reddit Data API** with OAuth (read-only scope).
5. **Commercial use, declared.** LeadFi is a for-profit company, so this is commercial use
   under Reddit's definition ("any use by a business"). Internal-only use and non-redistribution
   do not make it non-commercial, and we do not claim otherwise. Any access would operate only
   under whatever agreement Reddit grants.
6. Respect Data API rate limits; back off on errors. No unauthorized scraping, no circumventing
   access controls, no unofficial endpoints, and no acquiring Reddit content out of third-party
   search indexes or caches.

## Data use

7. **No redistribution.** Reddit content is never sold, licensed, republished, or otherwise
   redistributed.
8. **No model training.** Reddit content is never used as an input to train or fine-tune any AI
   or machine-learning model.
9. **Retention (design requirement, not currently running).** If the tool ever operated, every
   stored item would carry a `fetched_at` timestamp, raw content would be deleted after a fixed
   retention window, and nothing would be archived.
10. **Deletions (design requirement, not currently running).** If the tool ever operated, stored
    content would be re-checked against the API within each 48-hour window; content deleted or
    removed on Reddit would be hard-deleted from storage; no anonymized or de-identified copies
    of deleted content would be retained.

## No profiling, no individual-level use

11. **No profiling, no sensitive inference.** No user-level records; nothing is keyed by username
    or user ID. We do not derive, infer, score, or estimate any characteristic of any individual
    Redditor, financial or otherwise. We never attempt to re-identify or de-anonymize.
12. **Aggregate-only firewall.** Any insight from Reddit may inform aggregate messaging,
    positioning, objection language, and category understanding only. It must never flow into
    individual lead identification, enrichment, scoring, routing, or targeting. No username is
    ever stored alongside an inferred financial circumstance. Reddit data is never joined to the
    LeadFi product, to any customer or lead record, or to any credit or scoring system.
13. **No advertising use.** Reddit content is never used for ad targeting, audience building,
    lookalike modeling, or retargeting.
14. **No outreach.** We do not contact anyone based on what is read. Any Reddit participation by a
    LeadFi person is done by hand from a named, affiliation-disclosed account, outside this tool.

## Governance

15. Adding write access, automated posting, redistribution, or model-training use is out of scope
    and would require a separate reviewed decision and a separate agreement with Reddit.
