# hamray resource patch for Apktool M

This is a **branding-only preview** based on the supplied Exclave 0.17.66 decompiled APK snapshot. ByeDPI and WDTT are out of scope for this stage. This patch is not a compiled APK and does not change proxy/runtime behavior.

## Included

- `res/drawable-nodpi/hamray_icon.png`: the supplied black-and-white hamster artwork.
- `res/drawable-nodpi/hamray_monochrome.png`: monochrome silhouette for Android themed icons.
- `res/drawable/ic_launcher_foreground.xml`: adaptive icon foreground reference.
- `res/mipmap-anydpi-v26/ic_launcher.xml` and `ic_launcher_round.xml`: adaptive icon declarations.

## Apply in Apktool M

1. Back up the decompiled project.
2. Copy these files into the matching paths under `Exclave-0.17.66-arm64-v8a_src/res/`.
3. In `res/values/strings.xml`, set `app_name` to `hamray`. The default English value in the preview snapshot is already set this way.
4. Replace `ic_launcher.webp` and `ic_launcher_round.webp` in each `mipmap-mdpi`, `mipmap-hdpi`, `mipmap-xhdpi`, `mipmap-xxhdpi`, and `mipmap-xxxhdpi` directory with scaled exports of the supplied artwork. Keep both adaptive icon XML files consistent with the asset names.
5. Rebuild and install a test APK, then verify launcher masking on the actual device.

## Current limitations

The supplied archive contains DEX files but no decoded Smali or full Android Studio/Gradle project. This resource patch does not implement an in-app About screen, new navigation, connection-state animation, or proxy features. Material You behavior and the existing light/dark theme are preserved rather than reimplemented in this resource-only stage.

Do not treat this as a release-ready APK. Preserve the original Exclave notices and third-party licenses when redistributing.
