# VaultBytes OSS Stack

Open-source tools for testing, auditing, and explaining encrypted-inference systems built on Fully Homomorphic Encryption (FHE).

1. **FHE Oracle** — adversarial precision testing for FHE systems
2. **CipherExplain** — encrypted explainability under CKKS (BHDR is one kernel inside it; `bhdr-oss` is the open reference)
3. **Fairlearn-FHE** — encrypted fairness metrics
4. **RegAudit-FHE** — signed audit evidence for regulated AI
5. **FHE Attack Replay** — security regression testing for FHE configurations

## Where each tool fits

```
Encrypted inference system
        │
        ├── FHE Oracle: correctness / precision testing
        ├── Fairlearn-FHE: encrypted fairness metrics
        ├── CipherExplain: encrypted explainability
        ├── RegAudit-FHE: signed audit evidence
        └── FHE Attack Replay: cryptographic regression gates
```

## Repositories

| Tool | Repo |
|------|------|
| FHE Oracle | [fhe-oracle-oss](https://github.com/BAder82t/fhe-oracle-oss) |
| RegAudit-FHE | [regaudit-fhe](https://github.com/BAder82t/regaudit-fhe) |
| Fairlearn-FHE | [fairlearn-fhe](https://github.com/BAder82t/fairlearn-fhe) |
| CipherExplain — BHDR kernel | [bhdr-oss](https://github.com/BAder82t/bhdr-oss) |
| FHE Attack Replay | [fhe-attack-replay](https://github.com/BAder82t/fhe-attack-replay) |

## License

Each repository carries its own license. See individual READMEs for details.
