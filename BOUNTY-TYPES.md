# Bounty type guide

The [proposal](BOUNTY-PROPOSAL.md#phase-1-proposed-allocation) maps projects to these reusable briefs. Use the type’s task and checks, then agree the project inputs with the maintainer in the upstream issue.

## Maintainer bounties

For a new workflow, pin the supported release and link to a public entry point with setup, inputs, the command to run and the expected result. Deliver an upstream example and an executable check, plus matching guidance for [Cardano Dev Skills](https://github.com/cardano-foundation/cardano-dev-skills).

The reviewer should reproduce the result from a clean checkout using a local fixture or mock. Give two different coding agents the same entry URL and task prompt in fresh sessions. Record whether each agent found the instructions, ran the workflow and needed help.

For a follow-up, agree one changed input, version, runtime or service condition against a pinned baseline. Add a check for the expected result or diagnostic and update the relevant guidance. Use the project’s existing test entry point where practical.

### Validator tooling

- **Deliver** a small validator that compiles and runs against a known evaluation fixture.
- **Verify** the compile step and assert the declared evaluation result at the pinned version.
- **Follow up** by changing one compiler version or evaluation input and checking the expected result.

### Transaction and wallet SDKs

- **Deliver** a test ADA payment with a wallet or provider fixture. Supply an unsigned transaction when the SDK workflow starts at wallet or sponsorship integration.
- **Verify** the transaction recipient and lovelace amount and assert the result of the supported SDK step.
- **Follow up** by simulating one wallet, provider or sponsorship failure and asserting the result the caller receives.

### Transaction encoding and inspection

- **Deliver** an example that loads a known transaction or transaction body and reads one output through the public interface.
- **Verify** the recipient and lovelace amount against the fixture. Include a round trip or downstream check when it is part of the agreed scope.
- **Follow up** by checking the same fields or validation result at one other supported boundary, such as a browser binding, block reader or CLI.

### Chain data and indexing

- **Deliver** one versioned read query using a known address, transaction or UTxO.
- **Verify** the declared records or response fields against a deterministic fixture.
- **Follow up** by repeating the query under one controlled change and asserting the response, recovery or error.

### Local devnets

- **Deliver** a workflow that starts a pinned local devnet, checks readiness and exercises a test transaction.
- **Verify** readiness and that the transaction is visible through the supported query path.
- **Follow up** by changing one lifecycle or configuration condition and asserting the resulting status or transaction outcome.

## Shared DevX bounties

For shared workflows, agree the source or inputs, trigger, sample run, expected output and handover instructions. Use a saved fixture or replay where possible so reviewers can reproduce the result.

### Docs Drift

- **Deliver** a reusable check that compares guidance with an authoritative release and drafts a reviewable correction when it detects drift.
- **Verify** that it identifies the source and the mismatch and drafts the expected correction in sample runs for two projects.

### Protocol Parameter Alert

- **Deliver** a reusable alert triggered by a parameter change from an agreed authoritative source.
- **Verify** against a recorded change. The expected output gives the parameter, old and new values, effective epoch and source.

### Issue Triage

- **Deliver** a workflow that classifies issues and suggests where they should go for maintainer review.
- **Verify** the suggested classification, route and reason against agreed sample issues.

### Shared Workflow Check

- **Deliver** an optional follow-up that runs one common developer-task check against multiple projects.
- **Verify** that the output reports each result and identifies which step needs attention when a sample run fails.
