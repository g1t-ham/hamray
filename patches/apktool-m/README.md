# Apktool M resource patch

These are resource-level patch files, not a complete source project.

Copy the XML files into the matching paths under `Exclave-0.17.66-arm64-v8a_src/res/`. The source tree must also contain `res/drawable-nodpi/hamray_icon.png` and `res/drawable-nodpi/hamray_monochrome.png`, and all density-specific `mipmap-*/ic_launcher*.webp` files must be replaced by the supplied hamray icon variants.

In `res/values/colors.xml`, change `ic_launcher_background` to `#FF08080B` so the adaptive icon background matches the artwork.

In `res/values/strings.xml`, set `app_name` to `hamray`.

Before rebuilding, verify that the icon appears correctly on the device launcher. This patch does not add ByeDPI runtime integration or change connection behavior.
