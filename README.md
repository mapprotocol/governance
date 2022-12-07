# MGPs

MAPO’s Governance Proposals (MGPs) describe standard/issues/upgrades for the MAPO ecosystem, including the core protocol specifications, SDK, and contract standards. 

A MGP is a design document that should provide background information, a rationale for the proposal, detailed solution including technical specifications, a list of proposed changes and, if any, a list of potential risks. The proposer is responsible for soliciting community feedback and for driving consensus.



## Submitting MGPs
Draft all proposals following the template below and submit to the CIPs repository via a PR (pull request).

#### MGP template: ####

Please see [MGPs/mgp-template.md](MGPs/mgp-template.md) for a template.



## **Proposal Process**

Changes are managed via the MAP Governance smart contract. This contract acts as an "owner" for making modifications to other protocol smart contracts. Such smart contracts are termed **governable**. The Governance contract itself is governable, and owned by itself.

The change procedure happens in the following phases:

- Proposal

- Approval

- Referendum

- Execution

  

## Phases Overview

Each proposal starts on the **Proposal Queue** where it may receive **upvotes** to move forward in the queue relative to other queued proposals. Proposal authors should work to find community members to upvote their proposal (proposers may also upvote their proposals). Up to **3 proposals** from the top of the queue are dequeued and promoted to the approval stage automatically per day. Any proposal that remains in the queue for **4 weeks** will expire.

- **Approval** lasts **1 day (24 hours)**, during which the proposal must be approved by the Approver(s). Approved proposals are promoted to the Referendum stage.
- **Referendum** lasts **5 days**, during which owners of Locked MAP vote yes or no on the proposal. Proposals that satisfy the necessary quorum are promoted to the execution phase.
- **Execution** lasts up to **3 days**, during which anybody may trigger the execution of the proposal.

