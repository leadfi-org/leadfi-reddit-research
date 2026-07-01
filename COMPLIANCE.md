# Compliance policy

This tool is built and operated under the following hard rules. They are not optional and are
enforced in the tool's configuration and review process.

## Read-only

1. The tool uses **read endpoints only**. It never posts, comments, votes, messages, edits, or
   deletes anything on Reddit.
2. There is **no write access** on the app credentials, and there won't be under this app.
3. It is not a participant. It does not run automated replies or interact with users.

## Access

4. Access is through the **official Reddit Data API** with OAuth (read-only scope), requested
   through Reddit's standard process.
5. The tool respects Data API **rate limits** and backs off on errors.
6. No unauthorized scraping, no circumventing access controls, no use of unofficial endpoints.

## Data use

7. **Internal use only.** Reddit content and data are used for our own market and product
   research. We do not resell, license, republish, or otherwise redistribute it.
8. **No model training.** Reddit content is never used as input to train or fine-tune any AI or
   machine-learning model.
9. **Minimal retention.** We keep only what the research needs, and no longer than needed.
10. **Deletions honored.** When content is removed or deleted on Reddit, we remove it from our
    working data.
11. **No profiling.** We do not build profiles of individual users and we avoid collecting
    personal information.

## Governance

12. Any change that would add write access, automated posting, redistribution, or model-training
    use is out of scope for this tool and would require a separate, reviewed decision and, where
    applicable, a separate agreement with Reddit.
