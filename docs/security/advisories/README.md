# CodeIndexer security advisories

This directory archives the security advisories published for CodeIndexer, a proprietary MCP server distributed as binary releases. Each advisory describes a vulnerability that has already been fixed.

**The affected and fixed versions refer to CodeIndexer binary releases, not to the Markdown files in this repository.**

The advisories are also published at [codeindexer.dev/security/advisories](https://codeindexer.dev/security/advisories). These files are exported from the same data.

| ID | Title | Severity | Affected versions | Fixed | Published | Vendor advisory | GitHub advisory |
|---|---|---|---|---|---|---|---|
| [CI-SA-2026-001](CI-SA-2026-001.md) | Missing Host-header validation allowed DNS rebinding | High | v0.2.0 – v0.11.0 | First fixed version: v0.12.0 | 2026-10-21 | [codeindexer.dev](https://codeindexer.dev/security/advisories/ci-sa-2026-001) | [GHSA-c6vr-qp95-h5fr](https://github.com/Nettechnologys/codeindexer/security/advisories/GHSA-c6vr-qp95-h5fr) |
| [CI-SA-2026-002](CI-SA-2026-002.md) | Path traversal in the source-lines endpoint allowed arbitrary file read | High | v0.4.0 – v0.10.0 | First fixed version: v0.11.0 | 2026-10-21 | [codeindexer.dev](https://codeindexer.dev/security/advisories/ci-sa-2026-002) | [GHSA-jxhc-h8rv-2p75](https://github.com/Nettechnologys/codeindexer/security/advisories/GHSA-jxhc-h8rv-2p75) |
| [CI-SA-2026-003](CI-SA-2026-003.md) | Unvalidated project identifiers could escape the index root | High | v0.2.0 – v0.11.0 | First fixed version: v0.12.0 | 2026-10-21 | [codeindexer.dev](https://codeindexer.dev/security/advisories/ci-sa-2026-003) | [GHSA-w964-62f3-5735](https://github.com/Nettechnologys/codeindexer/security/advisories/GHSA-w964-62f3-5735) |
| [CI-SA-2026-005](CI-SA-2026-005.md) | Per-key project authorization was not enforced across MCP tools | High | v0.2.0 – v0.11.0 | Fully remediated in: v0.12.0 | 2026-10-21 | [codeindexer.dev](https://codeindexer.dev/security/advisories/ci-sa-2026-005) | [GHSA-43wx-76g7-9289](https://github.com/Nettechnologys/codeindexer/security/advisories/GHSA-43wx-76g7-9289) |
| [CI-SA-2026-009](CI-SA-2026-009.md) | Archive member paths could escape the extraction directory | Medium | v0.2.0 – v0.6.0 | First fixed version: v0.7.0 | 2026-10-21 | [codeindexer.dev](https://codeindexer.dev/security/advisories/ci-sa-2026-009) | [GHSA-499f-7wqh-526f](https://github.com/Nettechnologys/codeindexer/security/advisories/GHSA-499f-7wqh-526f) |

**Version identification:** Binaries of release v0.2.0 report version 0.1.0 (for example in `--version` output and in the MCP server information). Treat a build that reports 0.1.0 as affected; builds reporting 0.1.0 that predate release v0.2.0 were not assessed and must not be assumed unaffected. Applies to [CI-SA-2026-001](CI-SA-2026-001.md), [CI-SA-2026-003](CI-SA-2026-003.md), [CI-SA-2026-005](CI-SA-2026-005.md), [CI-SA-2026-009](CI-SA-2026-009.md).

These advisories document previously remediated vulnerabilities, consolidated for publication during an October 2026 retrospective review of CodeIndexer's development history. The review covered releases v0.2.0 through v0.12.0.

**Recommended upgrade:** v0.12.0 or later, which includes the fixes for every advisory currently published in this collection.

Severity uses a four-level scale — Critical, High, Medium, Low — judged by attacker reach, the required preconditions and the consequence. CVSS scores are not published. No CVE identifiers have been assigned.

To report a new vulnerability, see [SECURITY.md](../../../SECURITY.md).
