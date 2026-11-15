# User guide: Tally Commitments for Jira

Tally keeps track of what your team promised customers. It finds possible promises in Jira and
Confluence, lets a person confirm them, links each promise to the Jira work that delivers it,
flags risk with plain rules, and drafts customer updates that a person approves.

## 1. Install
1. Install Tally for **Jira** and for **Confluence** on the same site. Jira hosts the Tally
   page; the Confluence installation lets Tally quote and scan pages.
2. Open Tally from Jira: **Apps > Tally**.
3. Jira admins see **Load demo data** on the empty dashboard if you want to try it with a
   fictional dataset first.

## 2. Add accounts and commitments
- **Accounts:** a customer you make promises to. Add a name, tier and renewal date, and optionally
  the Jira project and Confluence space where that customer's work lives.
- **Log a commitment:** title, account, due date, and the evidence (a quote and its source).

## 3. Find promises automatically (Inbox)
1. Open **Inbox** and choose Jira projects and Confluence spaces to scan.
2. Tally reads issues and pages **as you** and lists possible promises with a suggested class
   (confirmed, possible, discussion, ambiguous) and any duplicate warning.
3. A person reviews each one: **Confirm**, **Edit and confirm**, **Mark ambiguous** or **Reject**
   (with a reason). Nothing is tracked until someone confirms it.

## 4. Deliver
- On a commitment, **Link issue** or **Create issue** to connect Jira work. Tally reads the live
  status: work in progress moves the commitment to In delivery; all linked issues Done moves it to
  Delivered.
- **Related context** shows parent, child, blocking and linked work from the Teamwork Graph, recent
  Confluence pages by the owner (**Attach as evidence**), and suggested owners when none is set.

## 5. Risk
Nine rules flag risk, each with a plain reason (for example "Due 5 Dec, DEMO-21 is blocked"):
overdue, due soon, no owner, no delivery work, blocked work, date mismatch, date moved, no
evidence, stale delivery. **Risks** groups them; **Acknowledge** hides a risk until a date you
choose, with a reason. Admins can change thresholds in **Settings > Risk rules**.

## 6. Customer updates
**Updates > New draft** (or **Draft customer update** on a commitment) writes an update from stored
facts only and shows the facts it used. Edit the wording, **Approve**, then **Copy text** into your
own email or chat and **Mark as sent**. Copy is disabled until approval; Tally never sends
anything. Marking sent moves delivered commitments it covers to Communicated.

## 7. Tally Agent in Rovo
In Rovo chat, choose **Tally Agent** and ask, for example: "Which commitments are at risk and why?",
"Which commitments have no owner?", "Draft a customer update for Acme Retail". Paste a message
from a customer and the agent proposes it to the Inbox for a person to review. The agent only
states facts Tally returns.

## 8. MCP tools for other AI assistants
Tally exposes seven tools through Atlassian's MCP server (Settings shows the URL). A site admin
must turn it on: **admin.atlassian.com > Apps > Sites > your site > Connected apps > Tally > View
app details > Expose tools to MCP-compatible apps**. Each user then signs in from their MCP client.
Note: external MCP clients reach the Confluence installation's copy of Tally data.

## 9. Settings
**Connections** checks Jira, Confluence and the Teamwork Graph as you. Admins edit **Risk rules**
and use **Data**: export everything as JSON, or delete all Tally data (type the site name to
confirm).

## 10. Uninstall and delete data
Before uninstalling, an admin can export and then delete all data in **Settings > Data**. Uninstall
from **Jira > Apps > Manage apps** (and from Confluence). See the privacy policy for what Atlassian
does with app data after uninstall.
