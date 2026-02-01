# How to Contribute to CMU Events API

## Did you find a bug, have an idea for a new feature, or any questions?

See [ScottyLabs Base Contributing Guide](https://github.com/ScottyLabs/wiki/wiki/Base-Contributing-Guide).

## Do you want to contribute to the codebase?

### Prerequisites

Because working on the Events API requires access to Carnegie Mellon University's event data,
you need to have an [Andrew ID](https://www.cmu.edu/computing/services/security/identity-access/account/userid.html).

### Do you want to process the scraped data?

#### Request Access

If you want to process and use the scraped data, follow the instructions in
[Governance](https://github.com/ScottyLabs/governance) to add yourself as a
[contributor](https://github.com/ScottyLabs/governance/blob/main/docs/contributors.md)
and join the [CMU Events API team](https://github.com/ScottyLabs/governance/blob/main/teams/events-api.toml)
as an applicant to request access to the scraped data.

You will have to work in a different ScottyLabs repository than this one.
**Make sure to describe your use case and link the corresponding repository in**
**the description of the PR in Governance.**

#### Development

Use the [S3 credentials](https://secrets.scottylabs.org/ui/vault/secrets/ScottyLabs/kv/list/events-api/)
to access the scraped data, process them, and perhaps store them in a database.

_Example use cases coming soon..._

#### Deployment

Deploy your service in Railway. Make a PR to this repository to update
[config.ts](../src/config.ts), which includes the Railway services the
event scraper will notify to restart their deployments after scraping the data.

#### Credited as a Contributor

Instead of submitting a PR, you will be
[credited as a contributor](https://github.com/ScottyLabs/wiki/wiki/PR-Process#credited-as-a-contributor)
after deploying a new live Events API serving processed scraped data.

### Do you want to scrape more data?

If you want to scrape more data, open an issue in this repository to discuss the
new data source you want to scrape. Once we have confirmed the new data source,
you can start working on the implementation.

Read the [ScottyLabs PR Process](https://github.com/ScottyLabs/wiki/wiki/PR-Process)
to familiarize yourself with the process of getting your changes merged and credited.

## Join Us! 🎉

We encourage you to get involved and join
[the team](https://github.com/ScottyLabs/governance/blob/main/teams/events-api.toml)!

Thanks! ❤️

CMU Events API Team
