# LeadFi Reddit Research (read-only)

An internal, **read-only** research tool that uses the official Reddit Data API to help
[LeadFi](https://leadfi.ai) understand the questions and problems people talk about around
financial readiness — things like soft credit checks, credit readiness, lead qualification,
and prequalification.

We read how real people describe these problems in their own words so our marketing and
product teams can write clearer, more accurate educational content and build something that
answers the questions people are actually asking.

**Status:** in development.

## What it does

- Reads public posts and comments from a focused set of finance, small-business, and sales
  subreddits (see `config.example.yaml`).
- Searches for public mentions of our company name so we can keep track of what people say
  about us.
- Summarizes the common questions, complaints, and wording people use, for our own internal
  research.

## What it does not do

- It does **not** post, comment, vote, or message anyone. It has no write access to Reddit and
  won't have any under this app.
- It is **not** a bot that participates in discussions, and it does not run automated replies.
- It only reads public data.

If someone from our team ever answers a question on Reddit, that's a real person doing it by
hand from a clearly identified account, with our affiliation stated up front. That happens
outside this tool.

## Data handling and compliance

- **Internal use only.** We don't resell, republish, or redistribute Reddit content or data.
- **No model training.** We do not use Reddit content to train or fine-tune any AI or
  machine-learning models.
- **Privacy.** We keep only what we need for the research, we don't build profiles of
  individual users, and we honor deletions and removals.
- **Rate limits.** We stay within the Data API rate limits and follow the Reddit Data API
  Terms and developer policies.

See [`COMPLIANCE.md`](./COMPLIANCE.md) for the full policy this tool operates under.

## How it accesses Reddit

Via the official Reddit Data API using OAuth with a read-only scope. Access is requested
through Reddit's standard API access process. No unauthorized scraping.

## Contact

hello@leadfi.ai · https://leadfi.ai
