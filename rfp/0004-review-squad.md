# RFP-0004: Review Squad

|                 |                                                                                                                  |
| --------------- | ---------------------------------------------------------------------------------------------------------------- |
| **Start Date**  | 2026/06/17                                                                                                       |
| **Description** | Establish a rotating Working Group of Fellows with maintainer status in `paritytech/polkadot-sdk` to provide sustained, incentivised PR review bandwidth for Fellowship members. |
| **Author**      | Pablo Andrés Dorado Suárez                                                                                       |


## Purpose and goals

The purpose of this RFP is to formalise a rotating **Review Squad** within the Polkadot Technical Fellowship: a bounded cohort of Fellowship members who hold active maintainer access to the [`paritytech/polkadot-sdk`](https://github.com/paritytech/polkadot-sdk) repository and who commit, for the duration of their rotation, to serving as primary reviewers and points of contact for pull requests authored by other Fellowship members.

### Rationale

Parity Technologies operates `paritytech/polkadot-sdk` with its own roadmap, release schedule, and internal reviewer pool. While Parity reviewers provide invaluable coverage, their availability is shaped by Parity's own priorities and is not guaranteed to align with the throughput needs of the broader Fellowship contributor base. This creates two recurring problems:

1. **Review latency**: PRs from Fellowship members can stall for extended periods, slowing down protocol work and discouraging contribution.
2. **Reviewer concentration**: A small set of Fellows who happen to be available absorb a disproportionate share of review load, risking burnout and creating single points of failure.

The Review Squad addresses both by:

- Providing a **predictable, dedicated review capacity** from within the Fellowship for Fellowship-member PRs.
- **Distributing the burden** across the membership through rotation, so no individual carries the load indefinitely.
- **Signalling value** through economic and/or social incentives, making the review function a recognised and rewarded Fellowship role rather than purely voluntary overhead.

> **Scope boundary**: this RFP covers reviews for PRs authored by *existing Fellowship members* (Ranks I–IX). A separate pipeline governs candidate support and external contributor onboarding.


## Budget and scope of work

### Squad composition

Each rotation will consist of **4–6 Fellows**, selected according to the criteria in the [Selection criteria](#selection-criteria) section. Squad size may be adjusted between rotations by the RFP proposer in response to demand and availability.

### Rotation period

Each rotation lasts **one calendar quarter (≈ 13 weeks)**. Members may re-apply for consecutive rotations but must be re-confirmed each time; the goal is sustained availability, not permanent appointment.

### Deliverables per rotation

Each Review Squad member is expected to:

1. **Maintain responsiveness**: provide an initial review or triage comment on any qualifying PR (see below) within **5 business days** of being assigned or tagged.
2. **Complete substantive reviews**: deliver thorough, actionable review feedback — not merely approval stamps — on a minimum of **8 qualifying PRs per month** across the squad (interpreted as a collective target, with individual contributions tracked).
3. **Serve as a point of contact**: be reachable on Matrix to answer architecture or integration questions from the PR author during active review cycles.
4. **Post a rotation report**: at the end of each rotation, each squad member submits a brief report (via a comment on this PR or a Subsquare post) summarising: number of PRs reviewed, notable technical decisions made during review, and any systemic bottlenecks observed.

A **qualifying PR** is any pull request to `paritytech/polkadot-sdk` (or its sub-repositories) where the author is a Fellowship member of Rank I or higher, or where the PR was formally referred to the Review Squad by an RFP-designated coordinator.

### Incentives

To recognise the additional commitment of serving on the Review Squad, participating members receive:

| Incentive type | Description |
|----------------|-------------|
| **Economic** | A per-rotation supplement paid from the Fellowship sub-treasury, budgeted at **$1,500 USD equivalent in DOT** per squad member per quarter (≈ $500/month). Payment is split into two tranches: 50 % at the start of the rotation and 50 % upon submission of the rotation report. |
| **Social** | Squad members are listed on the Fellowship website and in the Fellowship open channel announcement for the duration of their rotation. The rotation report is surfaced to the broader Fellowship as a standing agenda item. |

### Total budget estimate

Based on a squad of up to 6 members across up to 4 rotations per year:

| Item | Unit cost | Units | Total |
|------|-----------|-------|-------|
| Per-member quarterly supplement | $1,500 USD | 6 members × 4 rotations | $36,000 USD |
| Coordination overhead (see below) | $3,000 USD | 4 rotations | $12,000 USD |
| **Total (annual estimate)** | | | **$48,000 USD** |

A **coordinator role**, initially filled by the RFP proposer (Pablo Andrés Dorado Suárez) and transferable to any willing Fellow in subsequent rotations, handles scheduling, assignment of PRs to squad members, and rotation reporting logistics. The coordination supplement is $3,000 USD per rotation.

The Fellowship may adjust the number of active rotations per year or the squad size depending on on-chain treasury availability and observed demand.


## Useful resources

Prospective applicants should be familiar with the following:

- [`paritytech/polkadot-sdk`](https://github.com/paritytech/polkadot-sdk) — the primary repository covered by this RFP.
- [Polkadot Fellowship Manifesto](https://github.com/polkadot-fellows/manifesto) — governs Fellowship membership standards and expectations.
- [Polkadot Fellowship Runtimes](https://github.com/polkadot-fellows/runtimes) — Fellowship on-chain governance runtime.
- [Fellowship Salary pallet docs](https://docs.rs/pallet-salary/latest/pallet_salary/) — mechanism by which supplemental payments may be structured.
- [Polkadot Technical Fellowship Channel](https://matrix.to/#/#fellowship-members:parity.io) — primary async communication channel for Fellows.
- [Fellowship Open Channel](https://matrix.to/#/#fellowship-open-channel:parity.io) — public channel for announcements and PR referrals.


## Selection criteria

Applicants must meet **all** of the following requirements:

- **Fellowship membership**: active member of the Polkadot Technical Fellowship at Rank I (Dan) or higher at the time of application.
- **Maintainer access**: hold active maintainer or write access to `paritytech/polkadot-sdk` (or a substantive sub-repository thereof) at the time of application.
- **Review track record**: demonstrated history of substantive, technical PR reviews in `paritytech/polkadot-sdk` or closely related Substrate/Polkadot repositories within the 12 months prior to application. Applicants should provide a list of at least 5 reviewed PRs.
- **Availability**: able to commit to the responsiveness requirements above for the full duration of the rotation quarter. Members on a planned leave or with known competing commitments during the rotation period should defer to a subsequent rotation.

The following are desirable but not required:

- Experience reviewing PRs across multiple subsystems (consensus, networking, runtime, tooling).
- Prior participation in Fellowship governance (referenda voting, RFC authorship, Evaluation submissions).


## Application process

Applications are open to all eligible Fellowship members on a rolling, per-rotation basis.

### How to apply

1. **Prepare a short application** containing:
   - Your Fellowship rank and a link to your membership evidence.
   - Confirmation of active maintainer access to `paritytech/polkadot-sdk`.
   - A list of at least 5 PRs you have reviewed in the relevant repositories in the past 12 months (with links).
   - A brief statement (≤ 200 words) on your motivation and availability for the rotation.

2. **Submit your application** by opening an issue or posting a comment in the [Polkadot Technical Fellowship Channel](https://matrix.to/#/#fellowship-members:parity.io), tagging the RFP proposer. Applications must be received **at least 3 weeks before the start of the target rotation**.

3. **Review and selection**: the RFP proposer, in consultation with available Senior Fellows (Rank IV+), will shortlist applicants within one week of the application deadline. Selection prioritises diversity of subsystem expertise and avoids concentrating squad membership in any single organisation.

4. **Onboarding**: selected members are announced in the Fellowship channel and the Fellowship open channel. The RFP proposer schedules a brief kick-off call to align on tooling, triage process, and escalation paths.

5. **Payment**: the first tranche of the economic supplement is disbursed on-chain at the start of the rotation via the Fellowship sub-treasury. The second tranche is disbursed upon submission of the rotation report at the end of the quarter.

### Rotation schedule

| Rotation | Application deadline | Start date | End date |
|----------|---------------------|------------|----------|
| Q3 2026  | 2026/06/26          | 2026/07/07 | 2026/09/28 |
| Q4 2026  | 2026/09/11          | 2026/10/05 | 2026/12/21 |
| Q1 2027  | 2026/12/12          | 2027/01/05 | 2027/03/29 |
| Q2 2027  | 2027/03/13          | 2027/04/05 | 2027/06/28 |

**Note**: the first rotation (Q3 2026) is contingent on on-chain approval of this RFP. Subsequent rotation schedules will be confirmed or adjusted by the RFP proposer based on fellowship capacity and treasury availability.

### RFP completion

This RFP is considered complete when at least two full annual cycles (8 quarterly rotations) have been delivered, reported on, and reviewed by the Fellowship. At that point, the RFP proposer will post a final status comment on this PR and, if the programme is to continue, a successor RFP may be submitted incorporating lessons learned.
