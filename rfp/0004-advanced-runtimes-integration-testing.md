# RFP-0004: Advanced integration testing

|                 |                                         |
| --------------- | --------------------------------------- |
| **Start Date**  | 2025/03/02         |
| **Description** | Provide AI/Fuzzing guided integration tests for the *Polkadot Technical Fellowship* governed runtimes. |
| **Author(s)**   | Bastian Köcher                         |


## Purpose and goals

The runtimes governed by the *Polkadot Technical Fellowship* are built using FRAME. FRAME provides a lot of small components, the pallets, when combined together form a runtime.  
Each pallet is tested extensively via unit tests. However, the exact behavior of these pallets in the final runtime depends on their configuration in each runtime. So, integration tests are a must.
The runtimes themselves provide some integration tests, but their coverage is quite low. The [ecosystem tests](https://github.com/open-web3-stack/polkadot-ecosystem-tests) are integration tests
that are tailored for XCM, but could maybe also be extended for other use cases.

More integration tests are clearly needed—end user focused and security focused integration tests. End user focused integration tests should ensure that basic functionality, like sending some tokens,
is working as expected, while security focused integration tests should ensure that no combination of transactions can break any invariant of the runtime. While the former is a clear task of collecting
requirements and writing tests for these requirements, the latter is not that easy to achieve and requires more advanced integration tests that use fuzzing and/or AI.

So, the goal of this RFP is to provide end user and security focused integration tests.

## Budget and scope of work

200K USD worth of DOT, plus 200K USD worth of vested DOTs for bonus payments to be determined. The idea behind the bonus payment is that people doing an extraordinary job get properly rewarded.
It should also be prevented that potential security issues found by these tests are abused before being reported and fixed.

The scope of this RFP is:

- Tooling for writing integration tests
- Writing actual integration tests
- Integration into CI/long-running test jobs

Tooling should not be written for the sake of writing tooling. E.g., user-focused integration tests could be built on top of the ecosystem tests infrastructure.

## Useful resources

- [Testing: Staking Guardrails](https://github.com/polkadot-fellows/runtimes/issues/610)

## Application process

Applicants will need to:

1. Prepare an overview of their proposed work.
2. Reach out on the [Polkadot Technical Fellowship - Open Channel](https://matrix.to/#/#fellowship-open-channel:parity.io) to announce/discuss the proposal.
3. If shortlisted, liaise with Anaelle LTD to prepare a sub-treasury proposal detailing the tasks, costs, and timelines of each milestone. A generic template for Polkadot Treasury proposals is available [here](https://docs.google.com/document/d/1SQ3We_vLahpuLDg1op0ebr3C2CPwneEh2RlQduHfRVY/edit#heading=h.e126djyh5msy). 
4. Once finalised, publish the sub-treasury proposal as a discussion post on [Subsquare](https://collectives.subsquare.io/discussions) and announce the sub-treasury proposal in the [Fellowship Open Channel](https://matrix.to/#/#fellowship-open-channel:parity.io). After 14 Days, and provided there is no objection, the sub-treasury proposal will be submitted on-chain for voting. 
5. If approved, [claim the first tranche](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Fsys.ibp.network%2Fcollectives-polkadot#/extrinsics/decode/0x410600000000) of payment. 
6. Work on the sub-treasury proposal and post regular updates on the original discussion post on [Subsquare](https://collectives.subsquare.io/discussions). 
7. Submit a report for each stage of milestone completion to request the next tranche of payment, until the project is complete.



