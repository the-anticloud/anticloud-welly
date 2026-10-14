# Students — WELLY

**Project:** WELLY  
**Category:** OIL_GAS  
**Upstream:** https://github.com/agile-geoscience/welly  
**Pinned commit:** `6ed78b533ac7a5878bf7fd353d2b27ce3981b96a`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `6a3a2b9d0a737fd32cbffd70df10863fc1c26d06c6a07f072ae16b5b9b0edb88`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `6ed78b533ac7a5878bf7fd353d2b27ce3981b96a`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `6a3a2b9d0a737fd32cbffd70df10863fc1c26d06c6a07f072ae16b5b9b0edb88`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
