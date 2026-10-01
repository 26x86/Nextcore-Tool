# Historical public history handoff — nextcore-tool

## Current Status

The authoritative main at `49ab848e7c1c33c43e18c0a15886156dbf26924b` is the active module API. The older local public main `46969c53740f10e652c3306e6b818e8ecf56507c` and frozen source HEAD `4bb09da1243eba98ee8fb0ed01b58b3f36484209` contain 12 commit identities absent from that initial main ancestry. Ordinary local merge commits preserve those identities without replacing the current API or dependency pins. Publication must be verified separately.

## Target State

Keep the current module implementation active. Retain the distinct older conflict variants below as historical research source with their exact bytes, original paths, Git blob identifiers and SHA-256 hashes in [manifest.json](manifest.json). The preserved variants are unfinished historical work; their presence makes no compiler, runtime, operating-system boot, Metal or device acceptance claim.

## Conflict disposition

Current version, dependency revisions and repository publication schema are retained. Older Cargo and repository metadata variants are preserved here. The legacy main CLI source is byte-identical to the current main CLI source.

## License

Each recorded source revision includes its original `LICENSE.txt` in the manifest. The current module [LICENSE.txt](../../../LICENSE.txt) also remains unchanged.
