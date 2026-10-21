# Security Policy

CodeIndexer is proprietary software developed by NetTechnologys s.r.o.
This repository provides public documentation and security disclosures
for the CodeIndexer product. It does not contain the product source code.

## Reporting a vulnerability

Send sensitive reports through
[GitHub Private Vulnerability Reporting](https://github.com/Nettechnologys/codeindexer/security/advisories/new).

For initial, non-sensitive contact, email security@codeindexer.dev.
Request an encrypted channel before sending sensitive technical details
by email.

Do not disclose previously unreported vulnerabilities through public
issues or pull requests.

Please include:
- the product release and reported binary version, noting any discrepancy;
- the platform, relevant configuration and affected component;
- the required attacker capabilities and potential security impact;
- minimal reproduction steps or supporting evidence.

Remove live credentials, personal information and unrelated proprietary
data from reports.

We acknowledge reports within 48 hours. Remediation and disclosure timing
are coordinated with the reporter.

## Versions and security updates

CodeIndexer has publicly released binaries. Individual security advisories
document confirmed affected releases, available fixes and upgrade guidance.

Historical affected-version ranges describe vulnerability exposure, not
a maintenance or backport commitment. This policy does not promise fixes
for every historical release.

A version that is unlisted or not assessed must not be assumed unaffected.
Follow any version-identification notes in the relevant advisory.

## Security scope and trust boundaries

Relevant reports include failures of CodeIndexer security controls involving
untrusted repository contents, archives, browser-origin requests, network
clients, scoped API keys or agent-supplied tool arguments.

Local execution does not by itself make input trustworthy. Reports of
authentication bypass, authorization bypass, unintended filesystem access,
unsafe processing of untrusted input or other security-boundary violations
remain relevant on local installations.

An agent performing an explicitly permitted operation is not, by itself,
a CodeIndexer vulnerability. An agent-controlled tool call that bypasses
documented authorization or filesystem restrictions is relevant.

Reports that merely demonstrate capabilities an attacker already possesses
after compromising the host, without an additional privilege gain or
CodeIndexer security-boundary violation, are generally outside product
security scope.

Ordinary functional defects without security impact should be reported
through the regular issue tracker.

## Third-party dependencies

Report vulnerabilities in upstream components to their maintainers where
appropriate. Also notify us when a dependency vulnerability may affect
CodeIndexer, particularly when its use in the product creates a reachable
security impact.

A dependency finding is not excluded solely because the affected code is
maintained by another project.

## Responsible testing and disclosure

Use isolated installations and data you own or are authorized to test.
Avoid accessing other people's data or disrupting their systems.

This policy does not authorize testing customer deployments or production
services without permission from their owners.

We coordinate publication after assessing impact and remediation.
CVE identifiers may be requested when appropriate; assignment is not
automatic or guaranteed.

Reporter attribution is coordinated before publication, including requests
to remain anonymous. There is no paid bug-bounty offering.

## Published advisories

- [Vendor advisory index](https://codeindexer.dev/security/advisories)
- [Advisory archive in this repository](docs/security/advisories/README.md)
- [Security and responsible disclosure information](https://codeindexer.dev/security)

Commit references in advisories identify internal development history.
Their publication does not make the proprietary source code public.
