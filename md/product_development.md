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
- development happens in separate branches created from the "main" branch and called "*dev/TICKET_ID*".  `TICKET_ID` in this case is the ticket id of a `Story` or `Task`, never a `Sub-task`
- Developers will only work with `Sub-tasks` which are piece of work that need to be completed in order to complete its parent (`Story` or `Task`) ticket.  When development is completed for a `Sub-task`, developer must submit a pull request and mention the *`Sub-task` `TICKET_ID` as the title of the pull request* (By default, Github will take the first commit into your dev branch).
- The pull request will need to pass a set of preliminary automated tests and reviewed by a designated principal BDR developer before merging into `main`.

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

