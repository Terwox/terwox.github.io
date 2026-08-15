---
layout: bgg-hard-block
title: BGG Hard Block privacy policy
description: Privacy policy for the BGG Hard Block Chrome extension by Terwox.
permalink: /bgg-hard-block/privacy/
---

<p class="eyebrow">Effective August 15, 2026</p>

# Privacy policy

BGG Hard Block processes BoardGameGeek (BGG) data locally in the browser for one purpose: removing content from users the signed-in person has chosen to hide and, when enabled, keeping BGG's separate user subscription blocks aligned with that Hidden Users list.

The extension is inactive until the user reviews its in-extension disclosure and affirmatively agrees. If the disclosure changes, the extension requires agreement to the new version before processing BGG data again.

## Data handled

- BGG Hidden Users identifiers and the public BGG usernames associated with them
- discussion content and author attribution markup rendered on BGG forum indexes, forum threads, thumbs lists, GeekLists, images, videos, files, and individual blog posts
- reply-draft text BGG inserts into the editor after the user clicks Quote
- the current BGG page address, checked only in memory to enforce the supported discussion-page scope and never retained
- the signed-in BGG authorization value, used only in temporary page and background-worker memory to call BGG's own application programming interface (API)
- the user's subscription-linking preference and local status counts

The extension uses this data only to redact blocked author names on forum indexes and thumbs popovers; remove blocked posts, native blocked-user placeholders, quotations attributed to blocked users, and complete blocked-user quotation subtrees from BGG-generated reply drafts; report local removal/redaction counts; and, if the user leaves subscription linking enabled, add missing user-level subscription blocks to their BGG account. It never removes a subscription block.

## Data storage

The extension stores the user's consent record, blocked usernames, subscription-linking preference, synchronization and result status, local removal and redaction counts, and subscription-linking status in Chrome's local extension storage. It also stores a cache of blocked BGG profile identifier-to-public-username mappings there. It does not retain the address of the BGG page being viewed.

Profile-cache entries older than 30 days are never reused. A later successful synchronization removes those entries and any mappings whose identifiers are no longer in the current BGG Hidden Users result. Version 0.4.0 also removes the obsolete profile cache that earlier versions placed in BGG site `localStorage`, and rejects and removes unversioned block-list state written by the former page-data bridge.

Reply drafts are processed only in the currently open BGG page. The extension does not store them in Chrome extension storage, BGG local storage, or anywhere else.

The extension's filtering and BGG-data code is limited to canonical HTTPS addresses for those seven BGG discussion-page families. It does not activate filtering or credential capture on BGG's home page, game pages, collection, store, account pages, unrelated BGG pages, or any other site. After a single-page route leaves a supported page, a tiny local teardown function may run on the destination BGG page only to remove previously installed behavior; it reads no page data and makes no network request. Chrome treats host permissions as origin-wide even when URL paths are declared. The canonical BoardGameGeek origin is used to identify and attach code only on supported discussion pages. The canonical `api.geekdo.com` origin is used only for the Hidden Users, public-profile, current subscription-block, and optional subscription-block addition requests needed for the disclosed features.

The extension does not store the BGG `GeekAuth` authorization value. A document-bound capture returns it privately to the background worker, which uses it only during the current synchronization and then clears its reference. It is never exposed to the page's Document Object Model (DOM) or the isolated content script. The worker constructs only enumerated exact `https://api.geekdo.com` requests, refuses redirects, and does not accept API response data or request parameters from page code.

When the extension observes a native Hidden Users change, a data-free signal asks the background worker to pause optional subscription linking for that active document. This coordination is best-effort. The worker reads Hidden Users again immediately before each subscription addition, but Geekdo provides only a separate read and unconditional update with no conditional revision token. A native list change can occur between those requests, so the operation is not atomic.

## Data sharing

The extension has no analytics, advertising, telemetry, remote code, developer server, or third-party service. Terwox does not receive or have access to extension user data. Data is sent only to BGG/Geekdo endpoints that BGG's own frontend uses, over HTTPS, when necessary to provide the disclosed features.

## Limited use

BGG Hard Block's use of information complies with the Chrome Web Store User Data Policy, including the Limited Use requirements. Data is used only for the extension's disclosed single purpose. It is not sold, transferred to third parties, used for advertising or credit decisions, or made available for human review.

## Retention and deletion

Local extension data remains in the Chrome profile until Chrome clears it or the extension is removed. Cached BGG profile mappings older than 30 days are ignored and removed by the next successful synchronization, which also prunes mappings to identifiers in the current Hidden Users result. Removing the extension deletes its Chrome extension storage. Subscription blocks already written to the BGG account remain under the user's control in BGG's native subscription-block editor.

## Changes

Material changes to data handling will be disclosed inside the extension and will require fresh affirmative agreement before the changed practices begin.

## Contact

Questions about this policy can be sent to [terwox@gmail.com](mailto:terwox@gmail.com).
