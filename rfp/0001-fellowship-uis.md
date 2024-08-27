# RFP-0001: Fellowship UIs

|                 |                                                                                                                                   |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Start Date**  | 2024/08/27                                                                                                                        |
| **Description** | Design, build, and maintain a fit-for-purpose UI and UX to support all on-chain operations of the *Polkadot Technical Fellowship* |
| **Author**      | Anaelle LTD (on behalf of Gavin Wood & Bastian Köcher)                                                                            |


## Purpose and goals

The purpose of this RFP is to invite dapp developers to design, build, and maintain a fit-for-purpose UI and UX to support all on-chain operations of the Polkadot Technical Fellowship.

The primary goal is “*to enable Fellowship members and aspirational candidates to utilise and service this on-chain collective*”.



## Budget and scope of work

The total allocation available for this project is $500,000 USD.

This allocation is based on the following costs comparison for Fellowship UIs:

|Milestones |Polkassembly |Subsquare |RFP implementer (example)|
|-----------|-------------|----------|-------------------------|
|1          |$162,000 ([Finalised](https://docs.google.com/document/d/1lZGlBugwFcP_P5rfLpMyCFW49C_xqEkiFDA0zZETK3Y/edit#heading=h.dbbxpr5zj24u)) |$154,080 ([Finalised](https://polkadot.subsquare.io/referenda/631)) |$160,000 (Quantitative requirements 1-5) |
|2          |$140,400 ([Ongoing](https://docs.google.com/document/d/1cClkj64t-BC92MIV3-Fq696Ac5yUJHBnnJkBZR4tz70/edit#heading=h.bxakey85xitb)) |$144,000 ([Ongoing](https://polkadot.subsquare.io/referenda/1001)) |$35,000 (Qualitative requirements 1-4) |
|**Total**      |**$302,400** |**$298,080** |**$195,000** |

### Quantitative requirements:
The base scope of work for this project is described in the [Polkadot (Core) Fellowship UX Guidelines](https://hackmd.io/33pI3HvlSkycp-1dQjRLZA) and should cover the following on-chain modules (pallets):
1. [pallet_ranked_collective](https://docs.rs/pallet-ranked-collective/latest/pallet_ranked_collective/)
2. [pallet_referenda](https://docs.rs/pallet-referenda/latest/pallet_referenda/)
3. [pallet_core_fellowship](https://docs.rs/pallet-core-fellowship/latest/pallet_core_fellowship/)
4. [pallet_salary](https://docs.rs/pallet-salary/latest/pallet_salary/) 

An additional unit of work is the integration of the following on-chain modules:

5. [pallet_treasury](https://docs.rs/pallet-treasury/latest/pallet_treasury/)

### Qualitative requirements: 
The design and implementation of the UI should ensure the following:
1. Fellowship members are active in both reviewing the level of expertise of their peers and reporting these evaluations.
2. A system which enables a fluid and barrierless review-and-report cycle.
3. A UX that is sufficiently painless.

An additional but critical feature is:

4. A UI that displays stats for [specific voting activity](https://github.com/polkadot-fellows/Evidences/pull/40#discussion_r1668419965) so that the numbers are clear and voters can make a decision in line with the Manifesto.


## Useful resources
Prospective applicants can access and use the following resources to inform their work:
- [Polkadot (Core) Fellowship UX Guidelines](https://hackmd.io/33pI3HvlSkycp-1dQjRLZA)
- [Polkadot Technical Fellowship UX Audit Template](https://docs.google.com/document/d/1a6qe76yks2JKpjEjQY4WFxYApbAcaG4mJkEljoWn0hc/edit?usp=sharing)
- [Runtimes repo](https://github.com/polkadot-fellows/runtimes)
- [RFCs repo](https://github.com/polkadot-fellows/RFCs)
- [Evaluations repo](https://github.com/polkadot-fellows/Evaluations)
- [Polkadot Wiki - Polkadot Technical Fellowship](https://wiki.polkadot.network/docs/learn-polkadot-technical-fellowship)


## Selection criteria
Applicants should have extensive experience building intuitive dapps and/or UIs with relevant user documentation.

A working knowledge of the tools and libraries identified as [Fundamentals](https://github.com/polkadot-tooling-collective/collective/blob/master/mission_list.md) by the PoToC is also required.


## Application process
Applicants will need to:

1. Prepare an overview of their proposed product.
2. Reach out to Anaelle LTD on Matrix to discuss their proposed product before the final shortlisting.
3. If shortlisted, liaise with Anaelle LTD to prepare a sub-treasury proposal detailing the tasks, costs, and timelines of each milestone. A generic template for Polkadot Treasury proposals is available [here](https://docs.google.com/document/d/1SQ3We_vLahpuLDg1op0ebr3C2CPwneEh2RlQduHfRVY/edit#heading=h.e126djyh5msy). 
4. Once finalised, publish the sub-treasury proposal as a discussion post on [Subsquare](https://collectives.subsquare.io/discussions) and announce the sub-treasury proposal in the [Fellowship Open Channel](https://matrix.to/#/#fellowship-open-channel:parity.io). After 14 Days, and provided there is no objection, the sub-treasury proposal will be submitted on-chain for voting. 
5. If approved, [claim the first tranche](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Fsys.ibp.network%2Fcollectives-polkadot#/extrinsics/decode/0x410600000000) of payment. 
6. Work on the sub-treasury proposal and post regular updates on the original discussion post on [Subsquare](https://collectives.subsquare.io/discussions). 
7. Submit a report for each stage of milestone completion to request the next tranche of payment, until the project is complete.

**Important note: All milestones and deliverables must be completed within 3 months of the initial on-chain approval.**
