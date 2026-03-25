# Security Policy

## Supported Versions

Bullion256 is experimental software and is under active development.

Security fixes, if needed, are expected to apply to the current live public code and current public releases. Older builds, older release candidates, and unofficial repackaged binaries may not be supported.

If you are reporting a security issue, include the exact version, commit, release asset, and platform involved.

## Reporting a Vulnerability

If you believe you have found a security vulnerability in Bullion256, please do **not** open a public GitHub issue first for serious security problems.

Instead, report the issue privately to the project maintainer through the private contact method currently provided by the project.

If no dedicated private security contact is yet published, use the maintainer contact path already associated with the project and clearly mark the message as a **security vulnerability report**.

## What Should Be Reported Privately

Please report the following privately before public disclosure:

- consensus or block validation vulnerabilities
- wallet key handling issues
- seed, backup, restore, encryption, or unlock vulnerabilities
- transaction signing or spend authorization issues
- daemon or RPC authentication vulnerabilities
- remote crash, denial-of-service, or peer abuse issues
- mining or pool-related vulnerabilities that could affect network integrity
- installer, app bundle, or packaged wallet security issues
- vulnerabilities that could expose user funds, chain integrity, or network stability

## What to Include

Please include as much of the following as possible:

- affected version, release, or commit
- operating system and version
- whether the issue affects source builds, packaged releases, or both
- reproduction steps
- proof of concept, if available
- logs, screenshots, or terminal output, if relevant
- impact assessment
- whether the issue is reliably reproducible

Clear reports make triage and validation faster.

## Disclosure Expectations

Please allow reasonable time for the issue to be reviewed and, if necessary, fixed before public disclosure.

Public disclosure before a fix is available may place users, node operators, miners, or network infrastructure at risk.

Once an issue is understood and addressed, coordinated disclosure may follow.

## Scope Notes

Security-sensitive areas in Bullion256 include, but are not limited to:

- consensus logic
- wallet storage and recovery
- transaction creation and signing
- daemon startup and runtime behavior
- RPC access control
- peer-to-peer networking
- mining and pool interoperability
- packaged wallet releases and installers

## No Support Requests

This security policy is for vulnerability reporting only.

General wallet help, build help, node setup help, and mining support should be handled through the project’s normal public support or discussion channels rather than through a security report.
