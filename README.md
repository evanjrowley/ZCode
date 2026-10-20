# ZCode AppImage mirror

Holds the official ZCode Linux AppImage releases as release assets, so a Nix
flake can pin a `fetchurl` mirror that survives Z.ai removing old files from
its CDN.

Upstream: [zai-org/ZCode](https://github.com/zai-org/ZCode) (Apache-2.0).
This repository holds no source and no patch; each release on the
`appimage-v<version>` tag carries the byte-identical artifact that Z.ai's
CDN published, with its provenance in the release notes. To upgrade,
download the new AppImage from the CDN, hash it, and attach it to a new
`appimage-v<version>` release.
