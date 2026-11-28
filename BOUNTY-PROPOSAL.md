# Cardano DevX bounty proposal

Draft for maintainer review · 28 November 2026

Make common Cardano development tasks easier to find, run and verify. Phase 1 proposes one runnable workflow per selected project, plus two improvements that can serve multiple projects. A follow-up can test one distinct maintenance or compatibility case against the original workflow or an agreed baseline.

Use the same [bounty type guide](BOUNTY-TYPES.md) across projects. For example, off-chain SDKs use the same test ADA payment brief and review checks. Each maintainer fills in the supported version, fixture and SDK step when scoping the upstream issue.

## Phase 1 proposed allocation

| Project or shared proposal | Bounty type | Proposed USD |
| --- | --- | ---: |
| [Aiken](https://github.com/aiken-lang/aiken) | [Validator tooling](BOUNTY-TYPES.md#validator-tooling) | 1,250 |
| [OpShin](https://github.com/OpShin/opshin) | [Validator tooling](BOUNTY-TYPES.md#validator-tooling) | 1,250 |
| [Scalus](https://scalus.org/docs/get-started/ai-assisted-development) | [Validator tooling](BOUNTY-TYPES.md#validator-tooling) | 1,250 |
| [Evolution SDK](https://github.com/IntersectMBO/evolution-sdk) | [Transaction and wallet SDKs](BOUNTY-TYPES.md#transaction-and-wallet-sdks) | 1,500 |
| [UTxOS](https://github.com/utxos-dev/utxos-sdk) | [Transaction and wallet SDKs](BOUNTY-TYPES.md#transaction-and-wallet-sdks) | 1,500 |
| [Cardano Serialization Lib](https://github.com/Emurgo/cardano-serialization-lib) | [Transaction encoding and inspection](BOUNTY-TYPES.md#transaction-encoding-and-inspection) | 1,500 |
| [CQuisitor](https://github.com/cardananium/cquisitor) | [Transaction encoding and inspection](BOUNTY-TYPES.md#transaction-encoding-and-inspection) | 1,500 |
| [Pallas](https://github.com/txpipe/pallas) | [Transaction encoding and inspection](BOUNTY-TYPES.md#transaction-encoding-and-inspection) | 1,750 |
| [Yaci Store](https://github.com/bloxbean/yaci-store) | [Chain data and indexing](BOUNTY-TYPES.md#chain-data-and-indexing) | 1,500 |
| [Kupo](https://github.com/CardanoSolutions/kupo) | [Chain data and indexing](BOUNTY-TYPES.md#chain-data-and-indexing) | 1,500 |
| [Ogmios](https://github.com/CardanoSolutions/ogmios) | [Chain data and indexing](BOUNTY-TYPES.md#chain-data-and-indexing) | 1,500 |
| [Koios](https://github.com/cardano-community/koios-artifacts) | [Chain data and indexing](BOUNTY-TYPES.md#chain-data-and-indexing) | 1,500 |
| [Cardanoscan API](https://github.com/StricaHQ/cardanoscan-python) | [Chain data and indexing](BOUNTY-TYPES.md#chain-data-and-indexing) | 1,500 |
| Docs Drift | [Docs Drift](BOUNTY-TYPES.md#docs-drift) | 3,000 |
| Protocol Parameter Alert | [Protocol Parameter Alert](BOUNTY-TYPES.md#protocol-parameter-alert) | 3,000 |
| **Total** | **13 project proposals and 2 shared proposals** | **25,000** |

Project proposals total **US$19,000** and shared proposals total **US$6,000**. The US$1,250 project estimate assumes an existing fixture. US$1,500 covers a new fixture or an extra runtime check. US$1,750 includes downstream compatibility verification. Each proposed amount is subject to scope and funding approval.

## From proposal to issue

1. Confirm eligibility and a current gap. Use the scoring matrix to order eligible candidates and give priority to teams that have responded. Check that the proposed work is distinct from existing work or funded scopes.
2. Use the linked bounty type to agree the upstream issue, version, fixture, command and expected result. Record the problem, checks and definition of done. Get upstream maintainer confirmation and agree who will review the result independently.
3. Track each approved scope using the [Bounty issue template](.github/ISSUE_TEMPLATE/bounty.yml) and link the upstream issue that will host the bounty. Use the agreed checks to record delivery evidence.
