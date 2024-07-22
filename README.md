# RFPs
This repository contains a number of Requests for Proposals (RFPs) detailing specific tasks or projects needed to support the day-to-day operations of the Polkadot Technical Fellowship. These RFPs have been submitted for the sourcing and funding of new contributors/experts, as well as for the Fellowship's on-chain bodies to signal approval or disapproval of.


## Guidelines

The guidelines outline important information for the management of RFPs by RFP proposers and Fellowship members.

|Steps |Description |Participants |
|------|------------|-------------|
|1 |RFP proposer **drafts a new RFP** using the RFP template and **opens a PR in the `RFPs` repository on GitHub**. Fellowship members review the RFP. |RFP proposer, Fellowship members |
|2 |RFP proposer liaises with a Fellow or Architect to **submit the RFP for on-chain approval on the `Members` track** and **announces the proposal** in the Polkadot Fellowship-only channel. |RFP proposer, Rank 3+ members |
|3 |Fellowship **rejects/approves the RFP** through on-chain voting. |Fellowship members |
|4 |RFP proposer **announces the new RFP on Polkadot Forum** and in the Polkadot Fellowship open channel to formally invite applicants. |RFP proposer, builders |
|5 |RFP applicants **contact RFP proposer for feedback on their initial proposals**. RFP proposer **evaluates, shortlists, and rejects** initial proposals. |RFP proposer, RFP applicants |
|6 |RFP proposer liaises with RFP applicants to **draft or review their sub-treasury proposal** in line with the purpose, goals, budget, and scope of the RFP. |RFP proposer, RFP applicants |
|7 |RFP proposer **creates a discussion post on Subsquare** with the sub-treasury proposal document. Fellowship members review the sub-treasury proposal. |RFP proposer, Fellowship members |
|8 |RFP proposer liaises with a Fellow or Architect (if applicable) to **submit the sub-treasury proposal for on-chain approval on the `Fellows` or `Architects` track** and **announces the proposal** in the Polkadot Fellowship-only channel. |RFP proposer, Rank 3+ members |
|9 |Fellowship **rejects/approves the sub-treasury proposal** through on-chain voting. |Rank 3+ members |
|10 |RFP applicants are **officially onboarded as RFP implementers** and can claim their funding allocation to work on the RFP milestones. RFP proposer **liaises with RFP implementers through to the completion of the RFP milestones** and review their sub-treasury proposal report(s). |RFP proposer, RFP implementers |
|11 |RFP implementers **update the discussion post on Subsquare** with their sub-treasury proposal report(s). Fellowship members review the sub-treasury proposal report(s). |RFP implementers, Fellowship members |
|12 |RFP proposer **posts a comment on the status of the RFP on the PR in the `RFPs` repository on GitHub**. Fellowship members review the RFP status. |RFP proposer, Fellowship members |
|13 |RFP proposer **announces the completion of the RFP on Polkadot Forum** and in the Polkadot Fellowship open channel to formally close the RFP. |RFP proposer, builders |


## Process

The process for submitting RFPs is open to all existing Fellowship members (i.e Rank I to IX). Anyone may provide comments on submitted RFPs.

To submit an RFP, follow these steps:
  * Fork the `RFPs` repository.
  * Copy the `0000-rfp-template.md` file into the `text` folder and rename it to match the title of the RFP.
  * Fill out the RFP template and open a PR.

The Fellowship will decide, via an on-chain voting mechanism including all members, when to approve and merge RPCs. It does so by issuing an on-chain remark with the body RFP_APPROVE(xxxx, h) from the `Members` origin on the Polkadot Collectives blockchain, where xxxx is the number of the RFP and h is the blake2-256 hash of the raw proposal text. Once this remark has been approved, the PR can be merged. This on-chain process is designed to be resilient to where the RFPs are hosted and in what format, so it can be migrated away from GitHub in the future. The Fellowship should not approve more than one RFP with the same number.

The Fellowship may also decide to reject an RFP by issuing a remark with the text RFP_REJECT(xxxx, h). This is a formality to provide clarity on when PRs (or their analogue on non-GitHub platforms) may be closed. PRs may be closed by their author, as well. PRs may be closed when sufficiently stale, as well - after a period of 1 year without acceptance.


## Communication channels

The Fellowship is using Matrix for communication. Right now there exists two channels:

- [Polkadot Technical Fellowship Channel](https://matrix.to/#/#fellowship-members:parity.io): The channel for all Fellowship members to discuss. To get voice rights, you need to be part of the Fellowship. However, the channel is readable by anyone.
- [Polkadot Technical Fellowship - Open Channel](https://matrix.to/#/#fellowship-open-channel:parity.io): Open channel for anyone. Should be used to reach out to the Fellowship e.g. to request review or help on a topic.
