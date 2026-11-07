# Privacy Policy — Flow Explorer for Salesforce

_Last updated: November 7, 2026_

Flow Explorer for Salesforce ("the extension") is a browser extension that adds better search, filtering,
sorting and bulk actions to the **Setup → Flows** page of Salesforce orgs you are already logged in to.

**In short:** the extension talks only to the Salesforce org you are using. It has no servers of its own,
collects no analytics and does not sell, share or send your data anywhere else.

## What the extension accesses

| Data | Why | Where it goes |
|---|---|---|
| **Salesforce session cookie** (`sid`) for the org you are viewing | To call that org's Salesforce APIs (REST, Tooling and Metadata API) with your existing login, the same way the Salesforce UI does | Sent **only** to that same Salesforce org, as the authorization for its own API. It is never stored by the extension or sent anywhere else. |
| **Flow information** from your org (names, API names, types, objects, status, versions, last-modified user and date, descriptions) | To display, search, filter and sort your flows | Stays in your browser (in memory while the page is open). |
| **Flow contents** (element names and values from flow definitions) when you enable "Search inside flows" | To search inside flows | A compact search index is stored **locally** in your browser (`chrome.storage.local`) so it doesn't have to be downloaded again. |
| **Your preferences** (search text, filters, sort order, toggles) per org | To restore the view the next time you open it | Stored **locally** in your browser (`chrome.storage.local`). |

## What the extension does not do

- It does not send any data to the developer or to any third party. There are no analytics, tracking,
  advertising or crash-reporting services.
- It does not load or run code from remote servers.
- It does not read pages or sites other than Salesforce domains, and only shows its interface on the
  Setup → Flows page.
- It does not sell data, use it for advertising, or use it to determine creditworthiness or for lending.

## Changes made to your org

The extension changes your Salesforce org **only when you explicitly click** an action and confirm it:

- activating or deactivating flows,
- deleting obsolete flow versions.

These actions use your own Salesforce permissions. Salesforce rejects anything your user isn't allowed to do.

## Files you download

CSV and XML exports are created in your browser and saved through Chrome's normal download mechanism.
They are not uploaded anywhere.

## Data retention and removal

- The search index and preferences remain in your browser's extension storage until you remove the extension.
  Index entries for flow versions that no longer exist are cleaned up automatically.
- Uninstalling the extension deletes all data it stored.
- Nothing is retained anywhere else, because nothing is sent anywhere else.

## Chrome Web Store User Data Policy

The use of information received from Salesforce through this extension adheres to the
[Chrome Web Store User Data Policy](https://developer.chrome.com/docs/webstore/program-policies/user-data-faq),
including the Limited Use requirements.

## Trademarks

Salesforce and Flow Builder are trademarks of Salesforce, Inc. This extension is an independent project and is
not affiliated with, endorsed by, or sponsored by Salesforce, Inc.

## Changes to this policy

If this policy changes, the updated version will be published at this location with a new "Last updated" date.

## Contact

Questions about this policy: **sf.flow.explorer@gmail.com**
