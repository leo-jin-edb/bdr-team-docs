# Product development

## Versioning approaches

[Semantic versioning](https://semver.org/)

## Ways of working

The team adopts lean and devops methodologies, with peer reviews and a
multiple review workflow process. Kanban is used by the team to define
the tempo of development, with a prioritized backlog in Jira. Bi-weekly
sprint review meetings are held to provide status updates and determine
next goals.

## Development workflow

The workflow is based on the [*Github
Flow*](https://guides.github.com/introduction/flow/), with some
customizations:

- the Continuous Delivery branch is called "main" and is protected
- Github is configured for linear development (no merge commits)
- development happens in separate branches created from the "main" branch and called "*dev/TICKET_ID*"
- Once completed, developers must submit a pull request, which needs
  to pass some preliminary automated tests (\< 10 minutes) and then
  reviewed twice before being merged into "main" (with deeper
  automated tests required)

Automated tests vary in depth and width depending on the phase.
Scheduled tests run once a day or on demand for different Cloud
environments.

## Meetings

- Sprint kickoff
- Sprint review
- Daily standup

## Chats

Private chats: 

- [#eng-bdr-dev](https://edb.slack.com/archives/G01FLQYF0H1) - our private development channel

## Jira projects

- [*BDR (Bi-directional Replication)*](https://enterprisedb.atlassian.net/browse/bdr)

## Confluence space

- [*BDR Space*](https://enterprisedb.atlassian.net/wiki/spaces/BDR/overview?homepageId=1876590888)

