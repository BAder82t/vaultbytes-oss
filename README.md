# VaultBytes OSS Stack

Open-source tools for testing, auditing, and explaining encrypted-inference systems built on Fully Homomorphic Encryption (FHE).

This repository is the index. Each tool lives in its own repository with its own licence, issue tracker and release process.

## Which tool do I need?

| If you want to... | Use | Licence |
|---|---|---|
| find inputs where an encrypted program gives a different answer from its plaintext reference | [FHE Oracle](https://github.com/BAder82t/fhe-oracle-oss) | AGPL-3.0 |
| check that an FHE library returns correct results on every push, from CI | [VaultBytes Verify Action](https://github.com/BAder82t/verify-action) (private pilot, a token is needed) | no licence file yet, see its README |
| replay known attacks against your FHE configuration as a regression gate | [FHE Attack Replay](https://github.com/BAder82t/fhe-attack-replay) (also a [GitHub Action](https://github.com/marketplace/actions/fhe-attack-replay)) | Apache-2.0 |
| compute fairness metrics on encrypted predictions | [Fairlearn-FHE](https://github.com/BAder82t/fairlearn-fhe) | Apache-2.0 |
| produce signed, depth-tracked audit evidence for regulated AI | [RegAudit-FHE](https://github.com/BAder82t/regaudit-fhe) | AGPL-3.0, with a commercial licence |
| explain encrypted models (Kernel SHAP under CKKS) | [CipherExplain](https://vaultbytes.com/cipherexplain.html), whose BHDR regression kernel is open in [bhdr-encrypted-shap](https://github.com/BAder82t/bhdr-encrypted-shap) | AGPL-3.0, with a commercial licence |
| keep data and models private across organisations, with purpose-bound release and auditable evidence | [Encompute](https://github.com/BAder82t/Encompute) | AGPL-3.0 |

Licences above were read from each repository's `LICENSE` file. Each repository's own `LICENSING.md` or README is the authority, and it may change independently of this page.

## Where each tool fits

```
Encrypted inference system
        │
        ├── FHE Oracle / VaultBytes Verify: correctness and precision testing
        ├── FHE Attack Replay: cryptographic regression gates
        ├── Fairlearn-FHE: encrypted fairness metrics
        ├── CipherExplain (BHDR kernel): encrypted explainability
        ├── RegAudit-FHE: signed audit evidence
        └── Encompute: cross-organisation confidential computation and governance
```

## Pages on vaultbytes.com

- [FHE Oracle](https://vaultbytes.com/oracle.html)
- [VaultBytes Verify](https://vaultbytes.com/verify.html)
- [RegAudit-FHE](https://vaultbytes.com/regaudit-fhe.html)
- [CipherExplain](https://vaultbytes.com/cipherexplain.html) and the [BHDR note](https://vaultbytes.com/research-bhdr)

## Using these tools in CI

Pin any third-party Action, including ours, to a full commit SHA and not to a tag name, and give the workflow `permissions: contents: read`. The Verify Action documents this, the one host it contacts and how to check a release in its [SECURITY.md](https://github.com/BAder82t/verify-action/blob/main/SECURITY.md).

## Security reports

Report a vulnerability in a tool through that repository's `SECURITY.md` where it has one (Encompute, FHE Attack Replay, Fairlearn-FHE, RegAudit-FHE, VaultBytes Verify Action). For anything else, use the contact details at <https://vaultbytes.com>. Please do not open a public issue for a vulnerability.

## Licence of this repository

This index carries no code. Each tool's licence is stated in its own repository.
