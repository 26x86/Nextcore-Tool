# Nextcore-Tool

Command-line configuration validation, EFI bundle creation and recovery diagnostics.
This standalone crate pins Core and APLS to immutable Git commits. It requires
no sibling checkout; the integration workspace patches those URLs to its tracked
source snapshots during local development.

```sh
cargo test --all-targets
cargo run -- --help
```

EFI bundles accept a structurally validated x86_64 EFI image, including the
NXARMJIT image produced by Nextcore-EFI. ARM64e macOS targets an x86 computer;
the command-line tool is build/install orchestration, not the target JIT runtime.

Earlier release provenance is preserved in `repository.json`. Source/build tests
do not establish macOS boot or guest Metal acceleration.

## September 30 engineering snapshot

Current Status: This module is synchronized from one reviewed immutable integration snapshot. Its source revision and exact dependency pins are recorded in `repository.json`; file sizes and SHA-256 digests are recorded in `repository-files.json`. Existing repository history and license notices are preserved.

Target State: Independently reproducible source and module validation. Module tests establish the stated component behavior. macOS 27 boot and usable installed operation, guest Metal, physical installation and device qualification remain unverified.
