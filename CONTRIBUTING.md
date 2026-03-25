# Contributing to Bullion256

Thank you for your interest in contributing to Bullion256.

Bullion256 is a SHA-256 proof-of-work cryptocurrency project focused on transparent public source, node operation, wallet functionality, and mining infrastructure. Contributions are welcome from developers, testers, builders, infrastructure operators, and documentation contributors.

## Scope of Contributions

Contributions may include:

- core node and wallet improvements
- build and packaging improvements
- documentation updates
- platform compatibility fixes
- RPC, networking, or sync improvements
- mining and pool ecosystem support
- testing and reproducibility improvements
- release process improvements

## Before You Start

Please take time to review the repository structure and current project direction before opening a major change.

For larger or more sensitive changes, it is best to open an issue first so the change can be discussed before implementation begins.

This is especially important for changes affecting:

- consensus behavior
- proof-of-work logic
- block validation
- wallet safety or key handling
- transaction creation or signing
- RPC authentication or daemon startup behavior
- chain parameters
- mining compatibility
- release packaging and installer behavior

## How to Contribute

### Reporting Issues

If you find a bug, open an issue with as much detail as possible.

Helpful issue details include:

- what you expected to happen
- what actually happened
- operating system and version
- build method used
- relevant commands
- relevant logs or error output
- whether the problem is reproducible

If the issue may involve a security vulnerability, do **not** open a public issue first. Follow the process described in `SECURITY.md`.

### Submitting Pull Requests

Pull requests should be focused, clearly described, and limited in scope whenever possible.

A good pull request should include:

- a clear summary of what changed
- why the change is needed
- any important implementation notes
- testing performed
- platform or environment used for testing
- any known limitations or follow-up work

If your change affects user behavior, wallet behavior, RPC output, mining behavior, or release packaging, state that clearly in the pull request description.

## Coding Expectations

Please aim for changes that are:

- understandable
- minimal where practical
- well-scoped
- consistent with the surrounding codebase
- careful about backwards compatibility where relevant

Avoid mixing unrelated changes into a single pull request.

For sensitive areas such as consensus, wallet logic, and daemon behavior, smaller and more surgical changes are strongly preferred.

## Testing Expectations

When possible, contributors should test their changes before submitting.

Depending on the type of change, testing may include:

- successful rebuild from source
- daemon startup confirmation
- RPC sanity checks
- wallet creation and loading
- address generation
- peer connectivity checks
- mining-related behavior checks
- packaging/install verification on the target platform

If you were unable to test something, say so clearly.

## Build and Platform Notes

Bullion256 follows a Bitcoin Core style source layout and build flow, but contributors should avoid assuming that all upstream defaults or workflows apply unchanged.

When contributing build or packaging changes, please note the exact platform and method used.

Examples:

- Linux build environment
- macOS build environment
- wallet app packaging flow
- release archive generation
- installer or DMG behavior

## Documentation Contributions

Documentation improvements are welcome and important.

This includes:

- onboarding documentation
- build instructions
- wallet usage documentation
- mining setup guidance
- troubleshooting notes
- release notes
- operator guidance for nodes and infrastructure

Clear documentation reduces mistakes and improves trust in the project.

## Review and Acceptance

Opening a pull request does not guarantee acceptance.

Changes may be revised, narrowed, delayed, or declined based on project direction, safety concerns, maintenance burden, or compatibility impact.

Priority is generally given to changes that improve:

- correctness
- safety
- reproducibility
- clarity
- usability
- network reliability

## Conduct

Please keep contributions professional, technically grounded, and focused on improving the project.

Good-faith discussion, careful testing, and clear communication are expected.

## License

By contributing to Bullion256, you agree that your contributions will be licensed under the same license terms used by this repository.
