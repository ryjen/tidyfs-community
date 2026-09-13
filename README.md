# tidyfs-community

Public binary distribution surface for [tidyfs](https://github.com/ryjen/tidyfs).

This repository contains packaging metadata and public release artifacts only. It does **not** rebuild tidyfs or mirror its implementation source. The canonical `ryjen/tidyfs` repository remains the source, build, test, and release authority.

## Current release

- version: `0.7.0`
- canonical tag: `v0.7.0`
- canonical commit: `4ce8406a903ded92fcc3126933ac64aab700d626`
- target: `x86_64-unknown-linux-musl`
- archive: `tidyfs-0.7.0-x86_64-unknown-linux-musl.tar.gz`
- SHA-256: `fe818f3e609185e8af9dc9fd21f41e132fd42907168255c146c21dd73cd60bf9`

`release.json` is the machine-readable distribution identity. The community release asset must be byte-identical to the immutable canonical release asset. Nix consumption is pinned by cryptographic hash and must not require access to the canonical repository.

## Trust boundary

- this repository owns public packaging/distribution metadata, not product-version authority;
- release bytes are promoted without rebuilding or repacking;
- SHA-256 pinning proves byte identity/integrity, not reproducible-build or SLSA provenance;
- distributed binaries are assumed reverse engineerable and contain no secrets or hidden authorization material;
- rollback means pinning an earlier reviewed community packaging commit/release, never mutating an existing release identity.

## License

Apache-2.0 OR MIT, matching tidyfs.
