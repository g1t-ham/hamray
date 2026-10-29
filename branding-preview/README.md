# hamray branding preview

This branch contains a small, isolated launcher-branding patch for the supplied Exclave 0.17.66 decompiled APK snapshot. It is a preview, not a complete APK or a full source import.

## Included in this branch

- The supplied hamster artwork and a monochrome silhouette for themed launcher icons.
- Adaptive launcher icon XML for regular and round launchers.
- Apktool M instructions and explicit validation limits.

## Current scope

ByeDPI and WDTT are intentionally out of scope for now. This patch does not change proxy behavior, add app screens, or implement the planned “Тихий пульс” connection-state effect.

## Source and build status

The supplied archive contains DEX files but no decoded Smali or Android Studio/Gradle project. The local working copy has the app label set to `hamray` and launcher assets resized for mdpi through xxxhdpi; its ZIP integrity and edited XML were checked. It has not been rebuilt or installed on a device.

The complete decompiled archive has not been imported into this repository. Keep the original Exclave notices and third-party licenses if redistributing. Do not treat this preview as a release.

## Next safe steps

1. Review the icon on a real launcher and rebuild with Apktool M.
2. Confirm the app launches and existing light/dark behavior remains intact.
3. Only after the resource-only build is verified, plan the About screen and connection-state effect against the actual app structure.
