# tidyfs-community (deprecated)

This repository is retained only as a compatibility surface for existing pinned consumers and the historical immutable `v0.7.0` release.

Active tidyfs source, release, and binary-distribution work now lives in the public canonical repository:

- source and release authority: `ryjen/tidyfs`
- binary-oriented Nix flake: `distribution/`
- merged cutover commit: `8beca6cbcd9c732a712777a59a4dd46ae703906d`

New consumers should pin an exact reviewed `tidyfs` commit and select the distribution subflake:

```nix
tidyfs.url = "github:ryjen/tidyfs/8beca6cbcd9c732a712777a59a4dd46ae703906d?dir=distribution";
```

The historical files and release assets here are intentionally retained so existing locks such as `b6690394c15d4e666b26885d922414527e5c7d68` continue to resolve. No new releases should be promoted from this repository.

## Historical v0.7.0 identity

- canonical repository: `ryjen/tidyfs`
- canonical tag: `v0.7.0`
- canonical commit: `4ce8406a903ded92fcc3126933ac64aab700d626`
- target: `x86_64-unknown-linux-musl`
- archive SHA-256: `fe818f3e609185e8af9dc9fd21f41e132fd42907168255c146c21dd73cd60bf9`

## Status

Deprecated. Prefer `ryjen/tidyfs`. This repository may be archived once downstream references have been migrated; it should not be deleted while historical pinned consumers still depend on it.
