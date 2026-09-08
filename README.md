# Nextcore-Tool

Command-line configuration validation, EFI bundle creation and recovery diagnostics.
This standalone crate pins Core and APLS to immutable Git commits. It requires
no sibling checkout; the integration workspace patches those URLs to its exact
submodule versions during local development.

```sh
cargo test --all-targets
cargo run -- --help
```

EFI bundles accept a structurally validated x86_64 EFI image, including the
NXARMJIT image produced by Nextcore-EFI. ARM64e macOS targets an x86 computer;
the command-line tool is build/install orchestration, not the target JIT runtime.

Earlier release provenance is preserved in `repository.json`. Source/build tests
do not establish macOS boot or guest Metal acceleration.
