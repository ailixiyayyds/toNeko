# toNeko Minecraft 1.20.1 Backport

This repository is a public, community-maintained backport of the original
[CSneko/toNeko](https://github.com/CSneko/toNeko) project.

## Project status

- Target: Minecraft 1.20.1 with Fabric
- Upstream baseline: `V1.9.0` (`21790e31c6073bb941e6af1f0f2ecfa3c06ead2e`)
- Development branch: `1.20.1-backport`
- Status: early porting; Gradle dependency resolution is working, but source
  compilation is still blocked by 1.21-only component/network/recipe APIs.
- API reference: upstream tag `V1.3.9-1.20` is an actual Minecraft 1.20.1
  codebase and is used as a compatibility reference; it is not treated as the
  1.9.0 feature baseline.
- Relationship to upstream: unofficial; issues specific to this backport belong in this fork

The initial milestone is a Fabric client and dedicated server that build and
start on Java 17. NeoForge support is outside the first milestone.

The migration is being done in API groups (network payloads, entity data,
recipes, then client rendering) so the newer 1.9 feature set is preserved.

## License and attribution

The original project and this backport are licensed under GPL-3.0. Copyright
and attribution notices from upstream are retained. When distributing modified
binaries, distribute the corresponding source and GPL-3.0 license as required.
