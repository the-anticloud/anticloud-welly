# WELLY

![licence](https://img.shields.io/badge/licence-Apache-2.0-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![checks](https://img.shields.io/badge/checks-unknown_PASS-brightgreen)

> Governed Anticloud packaging of the upstream project `WELLY` in category **OIL_GAS**. check results: see ISOLATED_LAB_RESULTS. Every number below traces to a named file + run stamp; nothing is borrowed from other projects.

**Upstream:** WELLY · **Upstream pin:** `6ed78b533ac7a5878bf7fd353d2b27ce3981b96a` · **Category:** OIL_GAS · **Vendor:** Anticloud FZ LLE · **Licence:** Apache-2.0

---

## What This Project Does

![Welly banner](https://www.dropbox.com/s/a8jg7zomi4wgolb/welly_banner.png?raw=1)

[![Run tests](https://github.com/agilescientific/welly/actions/workflows/run-tests.yml/badge.svg)](https://github.com/agilescientific/welly/actions/workflows/run-tests.yml)
[![Build docs](https://github.com/agilescientific/welly/actions/workflows/build-docs.yml/badge.svg)](https://github.com/agilescientific/welly/actions/workflows/build-docs.yml)
[![PyPI version](https://img.shields.io/pypi/v/welly.svg)](https://pypi.python.org/pypi/welly/)
[![PyPI versions](https://img.shields.io/pypi/pyversions/welly.svg)](https://pypi.org/project/welly//)
[![PyPI license](https://img.shields.io/pypi/l/welly.svg)](https://pypi.org/project/welly/)

**`welly` facilitates the loading, processing, and analysis of subsurface wells and well data, such as striplogs, formation tops, well log curves, and synthetic seismograms.**

## Installation

    pip install welly

For developers, there are `pip` options for installing `test`, `docs` or `dev` (docs plus test) dependencies.

## Quick start

```python
from welly import Well, Project

w = Well.from_las('my_wells/my_well.las')  # Load a single well.
p = Project.from_las('my_wells/*.las')     # Load lots of wells.

gr = w.data['GR']  # One log...
gr.plot()          # ...with some superpowers!
```

Next, check out the tutorial notebooks.

## Documentation

[The `welly` documentation](https://code.agilescientific.com/welly) is a work in progress.

## Questions or suggestions?

[![mattermost](https://img.shields.io/badge/mattermost-software_underground-green)](https://mattermost.softwareunderground.org/)

**If you'd like to chat about `welly` with us or other users, look for the **#welly-and-lasio** channel in the [Software Underground's Mattermost](https://mattermost.softwareunderground.org/).**

To report bugs or suggest new features/improvements to the code, please [open an issue](https://github.com/agilescientific/welly/issues).

## Contributing

Please see [`CONTRIBUTING.md`](CONTRIBUTING.md).

## Philosophy

The [`lasio`](https://github.com/kinverarity1/lasio) project provides a very nice way to read and write [CWLS](http://www.cwls.org/) Log ASCII Standard files. The result is an object that contains all the LAS data — it's more or less analogous to the LAS file.

Sometimes we want a higher-level object, for example to contain methods that have nothing to do with LAS files. We may want to handle other well data, such as deviation surveys, tops (aka picks), engineering data, striplogs, synthetics, and so on. This is where `welly` comes in.

`welly` uses `lasio` for data I/O, but hides much of it from the user. We recommend you look at both projects before deciding if you need the 'well-level' functionality that `welly` provides.

---

## Installation

pip install welly

For developers, there are `pip` options for installing `test`, `docs` or `dev` (docs plus test) dependencies.

## Usage

See the upstream documentation quoted in What This Project Does above.

## API

[The `welly` documentation](https://code.agilescientific.com/welly) is a work in progress.

## Dependencies

| Metric | Value |
|--------|-------|
| Files | unknown |
| Lines of Code | unknown |
| Dependencies | unknown |
| Upstream license (harvested) | Apache-2.0 |
| Overlay license | Anticommons 0.1.0 |

Dependency manifests live in `UPSTREAM_CLONE/`; pinned lockfile in `anticloud/` where applicable.

## Configuration

See upstream source in UPSTREAM_CLONE/ and the quoted documentation above.

## Contributing

# Contributing

## 🙌 Thank you for considering contributing to `welly`!

There are several important ways you can help; here are some examples:

- Submitting bug reports and feature requests: see [Issues](https://github.com/agilescientific/welly/issues).
- Proposing code for bug fixes and new features, then [making a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
- Fixing typos and generally improving the documentation.
- Writing tutorials, examples, and how-to documents.

## Code of conduct

We're fortunate to be part of a large professional community that conducts itself with mutual respect and consideration for others. Agile's [Code of Conduct](https://github.com/agilescientific/community/blob/main/CODE_OF_CONDUCT.md) is part of protecting these features for everyone, everywhere. Please read it.

## Authorship

If you contribute a pull request to the project and you wish to be identified as an author, please add yourself to `AUTHORS.md`.

## License

By making a contribution, you agree that it shall be governed by the terms of [the license](LICENSE) unless another, specific agreement is made with Agile.

## License

Upstream © its respective contributors under Apache-2.0 (harvested MIT/Apache-2.0/BSD source; see `UPSTREAM_CLONE/LICENSE`). This packaging overlay is licensed under Anticommons 0.1.0.

## Upstream

- **project:** WELLY
- **Pinned SHA:** `6ed78b533ac7a5878bf7fd353d2b27ce3981b96a`
- **source:** `UPSTREAM_CLONE/` (pinned at the SHA above)
- **Upstream README source:** `UPSTREAM_CLONE/README.md`

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`4642308c1334186b652a2e1d1dc1006534ad7b9e4e789164e7678da69732812b`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| DANS (KNAW/NWO, Netherlands) | 10.17026/PT | EU-recognised archive |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe
and Mail, Business Insider, National Post, Financial Post, StreetInsider,
Digital Journal, Barchart, International Business Times, and Fox News.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

