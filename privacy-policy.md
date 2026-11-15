# Privacy policy: Tally Commitments for Jira

_Last updated: 16 November 2026_

Tally Commitments for Jira ("Tally") is an Atlassian Forge app published by Ifeoluwa Adegbulugbe
("we"). This policy explains what Tally stores, where, for how long, and how to delete it.

## Summary
- Tally runs entirely on Atlassian's Forge platform ("Runs on Atlassian"). It makes **no calls to
  servers outside Atlassian** and uses **no sub-processors**.
- Everything Tally stores lives in Forge storage inside your Atlassian site, in the same location
  as your Jira and Confluence data, and follows your site's data residency settings.
- We (the publisher) cannot see or access your data.

## What Tally stores
Only what your team creates or confirms in Tally:
- **Accounts:** customer account names, tier, renewal date, and optional Jira project and
  Confluence space keys.
- **Commitments:** title, due date, status, priority, owner (an Atlassian account ID), linked Jira
  issue keys, and a version history (who changed what and when, by Atlassian account ID).
- **Evidence quotes:** short quotes (up to 300 characters) copied from Jira issues or Confluence
  pages, with a link to the source. Email addresses in quotes are masked before saving.
- **Discovery candidates:** possible promises found when a person runs a scan of the Jira projects
  or Confluence spaces they choose, or proposes one through the Tally Rovo agent, waiting for
  human review.
- **Risk signals:** which built-in rule fired for a commitment and why.
- **Issue snapshots:** status, assignee account ID, due date and last-updated time of linked Jira
  issues, used to evaluate risk rules.
- **Customer update drafts:** the draft text, who approved it, and who marked it sent, with times.
- **Settings:** risk rule thresholds and similar configuration.

Tally does **not** store passwords, API tokens, payment details, or user email addresses. User
display names are read from Jira when a page is shown and are not stored.

## How Tally reads your data
All Jira, Confluence and Teamwork Graph requests run **as the signed-in user**, so Atlassian's own
permissions apply: Tally can only read what that person can already see.

## Rovo agent and MCP
Tally includes a Rovo agent and Atlassian MCP tools. When someone uses them, Tally returns
commitment data to Atlassian Rovo, which is covered by Atlassian's own terms. If a site admin turns
on external MCP access, an MCP client that a user connects (for example, an AI assistant) receives
the tool results that user requests. Tally never contacts customers and never sends messages.

## Logs
Tally writes one line per request to Atlassian's Forge logs: the action name, an outcome code and
a duration. Logs contain no commitment text, quotes or customer data. Atlassian shows Forge logs to
the publisher for 30 days.

## Retention and deletion
- Data stays until your team deletes it.
- A Jira admin can delete **all** Tally data on the site at any time: Tally > Settings > Data >
  Delete all data. Admins can also export everything as JSON first.
- When the app is uninstalled, Atlassian soft-deletes its data and removes it according to
  Atlassian's Forge hosted storage data lifecycle. If the app is reinstalled within 21 days,
  Atlassian may relink the previous data.

## Your rights
Because the data stays inside your Atlassian site, your site admins control it. For questions
about this policy, contact ifeoluwaadegbulugbe@gmail.com.

## Changes
We will update the date above when this policy changes.
