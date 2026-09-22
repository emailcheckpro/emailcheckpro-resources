# EmailCheckPro resources

Official technical resources, guides and developer articles for **EmailCheckPro** — email deliverability and email avatar checks.

- **Website:** https://emailcheckpro.com
- **Blog:** https://emailcheckpro.com/blog
- **API documentation:** https://emailcheckpro.com/api-docs
- **Pricing:** https://emailcheckpro.com/pricing

## What is in this repository

This repository is the public home for EmailCheckPro technical writing that is published outside the website:

- **[Issues](../../issues)** — short technical notes on integration, result interpretation and operational practice.
- **[Discussions](../../discussions)** — longer announcements and product guidance under the *Announcements* category.

The canonical version of every product fact lives on the website. Where an article and the site disagree, the site wins.

## Official API example repositories

One repository per product, each with an OpenAPI contract, a machine-readable `product.json`, an `llms.txt` summary and runnable examples in seven languages.

| Product | Shape | Repository |
|---|---|---|
| [Email Deliverability Check](https://github.com/emailcheckpro/email-deliverability-checker-api) | Realtime | `email-deliverability-checker-api` |
| [Email Avatar Check](https://github.com/emailcheckpro/email-avatar-checker-api) | Realtime | `email-avatar-checker-api` |
| [Email Bulk Avatar Check](https://github.com/emailcheckpro/email-bulk-avatar-api) | Bulk (async) | `email-bulk-avatar-api` |
| [Email Bulk Deliverability Check](https://github.com/emailcheckpro/email-bulk-deliverability-api) | Bulk (async) | `email-bulk-deliverability-api` |

A **realtime** check answers inside the same HTTP response (`POST /api/v1/check`, or `POST /api/v1/batch-check` for up to 100 identifiers). A **bulk task** takes a file and answers later (`POST /api/v1/bulk-tasks`). They are separate endpoints and are not interchangeable.

## Responsible use

EmailCheckPro results are **point-in-time signals**. A result describes what a provider reported at the moment of the check — it is not identity verification, not proof of ownership, and not permission to contact anyone. Use the API only for identifiers you are authorized to process, and comply with applicable privacy laws and platform terms.

Third-party trademarks belong to their respective owners; no affiliation or endorsement is implied.

---

*Maintained by EmailCheckPro. Questions and integration problems: https://emailcheckpro.com/contact*
