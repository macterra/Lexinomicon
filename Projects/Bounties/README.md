# Bounties

1. Bounties provide a mechanism for funding tasks. 
1. Tasks are tracked as [Lexinomicon issues](https://github.com/ulex-opensource/Lexinomicon/issues).
1. The bounty MUST get its own page which includes:
* name (Bounty-#) where # is the issue #
* associated issue link
* lead [Gatekeeper](../../Roles/Gatekeeper)
* lead [Keymaster](../../Roles/Keymaster)
* assigned [Treasurer](../../Roles/Treasurer)
* associated project link
* requirements
* estimate
* funding deadline
* bounty address 
* deliverables

## Process

The players involved SHOULD marshal the bounty through the following standard stages in the [Bounties project](TBD):

### Triage

1. The bounty's wiki page and corresponding issue are created and cross-linked.
1. Requirements (acceptance criteria) are managed by the Gatekeeper.
1. An estimate (from the table below) is provided by the Keymaster.
1. The Gatekeeper and Keymaster negotiate requirements and estimates until they come to a common understanding.
1. When ready the Gatekeeper moves the issue to `Proposed` and hands off (assigns the issue) to the Treasurer.

### Proposed

1. The Treasurer reviews the bounty's market value against comparable work in other markets. If out of line the Treasurer SHOULD send the issue back to `Triage`.
1. The Treasurer creates a crowdfund page on the pay server and publishes the corresponding link on the wiki page.
1. The Treasurer notifies subscribers that the bounty is open for funding.
1. The Treasurer monitors the funding and periodically notifies subscribers of progress.
1. If the bounty funding reaches 100% the Treasurer is responsible for:
    1. moving the issue to `In Progress`,
    1. updating the wiki page,
    1. recording who owns how many shares in the bounty by percentage funded,
    1. handing off to the Keymaster.
1. If the deadline is reached before the bounty is funded the Treasurer is responsible for:
    1. sending refunds to participants, 
    1. updating the wiki page,
    1. closing the issue.

### In Progress

1. The Keymaster is responsible for delivering on the requirements.
1. The Keymaster should periodically update the issue with progress reports.
1. After the bounty is funded the requirements and/or estimate MAY only be updated if both the Gatekeeper and Keymaster approve the changes.
1. When ready the Keymaster updates the Deliverables section of the wiki page, moves the issue to `In Review`, and hands off to the Gatekeeper.

### In Review

1. The Gatekeeper is responsible for testing deliverables against requirements.
1. The Gatekeeper opens separate issues for any deltas found, moves the bounty issue back to `In Progress` and hands off to the Keymaster.
1. If the requirements are all satisfied the Gatekeeper moves the issue to `Complete` and hands off to the Keymaster and Treasurer.

### Complete

1. The Keymaster creates a payment request in the pay server and sends a link directly to the Treasurer.
1. The Treasurer verifies the request then marshals a [1S/1V](../../Process/Voting/Double-Democracy) vote for bounty share-holders to release the funds.
1. If the vote fails the Treasurer hands off to the Gatekeeper for another iteration of `In Review`.
1. If the vote passes the Treasurer sends the payment to the Keymaster.
1. When the payment is received the Keymaster closes the issue.

## Estimates

1. The Treasurer is responsible for periodically adjusting bounty sizing estimate table.
1. The Gatekeeper and Keymaster can request an update to the estimate table at any time.

| size | time (hours, P50/P90) | bounty (BTC) | 
| ---- | ----- | ----- |
| S    |  5/10 | 0.125 |
| M    | 10/20 | 0.250 |
| L    | 20/40 | 0.500 |
| XL   | 40/80 | 1.000 | 
