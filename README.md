# PermitSeal

**Local-first permit, inspection, and approval evidence sealer for field operators.**

Offline. Deterministic. Pay once. Compatible with QuantumGuard CONTRACT-v1 and the Operator Pages suite.

## Why PermitSeal?

Missing permits, failed inspections that get "lost," or "we never approved that" disputes delay projects and create liability.  
PermitSeal captures structured permit and inspection records (IDs, authorities, results, conditions, inspectors, notes, media hashes) and seals them into a client-verifiable QuantumGuard evidence bundle.

- No SaaS. No subscription. Runs completely offline after key setup.
- Clients (or auditors / AHJs) verify with free QuantumGuard verifier (`qg verify`).
- Deterministic: same inputs → same sealed pack.
- Pairs with DailySeal, SafetySeal, ChangeOrderSeal, BinderSeal, and the rest of the Operator Pages suite.

## Quick Start

```bash
pip install cryptography

python3 src/permitseal.py --demo
python3 src/permitseal.py --json samples/permit-001.json --out sealed-permit.json
```

Verify:
```bash
qg verify sealed-permit.json
```
Expected: **PASS**.

## What you can sell

| SKU       | Price | Includes                                      |
|-----------|-------|-----------------------------------------------|
| Operator  | $49   | CLI + sample templates + key setup guide + 1-year email support |
| Command   | $149  | + batch mode + CSV/HTML export + reseller rights |
| Agency    | $399  | + white-label + multi-site key management |

**Buy Operator Pack:** [Test checkout](https://buy.stripe.com/test_bJe8wO1Cz0SIcxG4Gsew806) or contact for live.  
Contact: danpennic@gmail.com  
Repo: https://github.com/danpennic-sys/permitseal

Source free under Apache-2.0 OR MIT. Commercial packs sold separately.

## License

Apache-2.0 OR MIT
