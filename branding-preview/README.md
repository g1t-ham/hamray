# hamray branding preview

This directory contains the first isolated branding asset for review. It is not a complete APK or a full Exclave source tree.

## Included

- `hamray_icon.png`: compact preview/export of the supplied hamster avatar.

## Intended Android resource locations

The icon should be reviewed against the original artwork before use as the app launcher icon. The final Apktool M resource update should replace all density-specific launcher assets and preserve the adaptive icon XML structure. Do not replace the original vector/XML blindly without checking how the icon is masked on Android launchers.

## Current status

This is an isolated preview branch. The full decompiled archive has not yet been imported into this repository. The supplied archive contains DEX files but no decoded Smali source or Android Studio/Gradle project, so it is not yet a complete, rebuildable source project.

The planned next steps are to import the source snapshot safely, apply branding across all icon densities, verify the app label and themes, then implement and test ByeDPI profile support. WDTT is out of scope.
