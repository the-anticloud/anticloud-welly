# Educators — WELLY

**Project:** WELLY  
**Category:** OIL_GAS  
**Upstream:** https://github.com/agile-geoscience/welly  
**Pinned commit:** `6ed78b533ac7a5878bf7fd353d2b27ce3981b96a`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `6a3a2b9d0a737fd32cbffd70df10863fc1c26d06c6a07f072ae16b5b9b0edb88`  
**Date:** October 2026

## Teaching with WELLY

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `6a3a2b9d0a737fd32cbffd70df10863fc1c26d06c6a07f072ae16b5b9b0edb88` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
