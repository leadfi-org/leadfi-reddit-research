# LeadFi Reddit Research

> **Status: not operational.** LeadFi applied for read-only access to the official
> Reddit Data API for the research described below, and **that access was not granted.**
> As a result this tool is not running, it accesses no Reddit data, and it stores no
> Reddit data. This repository documents the intended read-only design and the
> compliance posture we committed to. Nothing here touches Reddit today.

[LeadFi](https://leadfi.ai) is a for-profit company working in financial-readiness lead
qualification. This tool was designed to help our marketing and product teams understand
how people describe problems around things like soft credit checks and credit readiness,
so we could write clearer, more accurate educational content.

## What it was designed to do

If read-only Data API access were ever granted under an appropriate agreement with Reddit,
the tool was designed to:

- Read public posts and comments from a focused set of finance, small-business, and sales
  subreddits (see `config.example.yaml`).
- Note public mentions of the company name.
- Summarize recurring questions, complaints, and the wording people use, for our own
  internal research.

It was designed to be strictly read-only. It has no write capability.

## What it does not do (and would not do)

- No posting, commenting, voting, or messaging. No write access.
- No reselling, licensing, republishing, or redistributing Reddit content or data.
- No using Reddit content to train or fine-tune any AI or machine-learning model.
- No profiling of individual users, and no deriving or inferring sensitive characteristics
  about anyone.

Any Reddit participation by a LeadFi person is done by hand, from a named account that
states the LeadFi affiliation, entirely outside this tool.

## Commercial use, stated plainly

LeadFi is a business, so this would be commercial use under Reddit's definition ("any use
by a business"). Internal-only use and not redistributing data do not make it
non-commercial, and we do not claim otherwise. Any future access would run only under
whatever agreement Reddit grants.

## Design commitments

The rules the design commits to are in [`COMPLIANCE.md`](./COMPLIANCE.md). They describe
intended behavior, not a running system. The most important one: any insight from Reddit
would inform **aggregate** messaging and category understanding only. It would never flow
into identifying, enriching, scoring, routing, or targeting an individual person, and no
username would ever be stored alongside an inferred financial circumstance.

## Contact

https://leadfi.ai
