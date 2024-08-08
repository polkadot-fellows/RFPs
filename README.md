# RFPs
This repository contains a number of Requests for Proposals (RFPs) detailing specific tasks or projects needed to support the day-to-day operations of the Polkadot Technical Fellowship. These RFPs have been submitted for the sourcing and funding of new contributors/experts, as well as for the Fellowship's on-chain bodies to signal approval or disapproval of.


## Guidelines

RFP proposers can find mportant information for the management of RFPs [here]().


## Process

The process for submitting RFPs is open to all existing Fellowship members (i.e Rank I to IX). Anyone may provide comments on submitted RFPs. 

To submit an RFP, follow these steps:
  * Fork the `RFPs` repository.
  * Copy the `0000-rfp-template.md` file into the `rfp` folder and rename it to match the title of the RFP.
  * Fill out the RFP template and open a PR.
  * Announce the RFP to the Fellowship and wait at least one week.
  * If there are no major pushbacks by the Fellowship, the RFP can be put to a vote.

The Fellowship will decide, via an on-chain voting mechanism including all members, when to approve and merge RFPs. It does so by issuing an on-chain remark with the body RFP_APPROVE(xxxx, h) from the `Members` origin on the Polkadot Collectives blockchain, where xxxx is the number of the RFP and h is the blake2-256 hash of the raw proposal text. Once this remark has been approved, the PR can be merged. This on-chain process is designed to be resilient to where the RFPs are hosted and in what format, so it can be migrated away from GitHub in the future. The Fellowship should not approve more than one RFP with the same number.

The Fellowship may also decide to reject an RFP by issuing a remark with the text RFP_REJECT(xxxx, h). This is a formality to provide clarity on when PRs (or their analogue on non-GitHub platforms) may be closed. PRs may be closed by their author, as well. PRs may be closed when sufficiently stale, as well - after a period of 1 year without acceptance.


## Communication channels

The Fellowship is using Matrix for communication. Right now there exists two channels:

- [Polkadot Technical Fellowship Channel](https://matrix.to/#/#fellowship-members:parity.io): The channel for all Fellowship members to discuss. To get voice rights, you need to be part of the Fellowship. However, the channel is readable by anyone.
- [Polkadot Technical Fellowship - Open Channel](https://matrix.to/#/#fellowship-open-channel:parity.io): Open channel for anyone. Should be used to reach out to the Fellowship e.g. to request review or help on a topic.
