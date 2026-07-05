# Unofficial Blender for iPad / iOS (sideload build)

> ⚠️ **Unofficial community build. NOT affiliated with, endorsed by, or supported by the Blender Foundation.**
> Pre-alpha, experimental build of Blender's in-progress iOS port. Expect bugs and crashes.

Automated GitHub Actions pipeline that compiles Blender's experimental `ios` branch into an
unsigned `.ipa` you can sideload onto an iPad — no Mac required.

## Install

1. Download the latest `Blender-ios.ipa` from the [**Releases**](../../releases) page.
2. Open a sideloading tool (**Sideloadly**, **AltStore/SideStore**, or **Impactor**) on your PC and connect the iPad.
3. Load the IPA, sign in with your Apple ID, and install.
4. On the iPad: **Settings → General → VPN & Device Management → trust your developer certificate**.
5. Launch Blender.

Free Apple ID note: the app expires after **7 days** (just re-sideload).

## What you need

- iPad, Apple-silicon (M1+) strongly recommended
- Windows/macOS/Linux PC for sideloading
- Free or paid Apple ID + a sideloading tool

## Fixes included in this build

- Hardware keyboard shortcuts (layout-aware, via `GCKeyboard`)
- Magic Keyboard trackpad support (click/drag, pinch-zoom, scroll navigation)
- Slider/number-field scrubbing via pointer drag
- Direct in-place text editing with a hardware keyboard attached
- Native iOS file picker for open/save/import/export
- Fix for a startup crash (`wm_add_default` null pointer)
- Back button for secondary windows
- Console logging to `blender_input.log` / `blender_console.log` for debugging
- App icon

## Known limitations

- May crash on launch or during use
- Keyboard/trackpad support is partial
- Add-ons / Extensions platform do not work
- No official support

## License

Blender is **GNU GPL**. This build modifies Blender; corresponding source is the upstream
`ios` branch at <https://projects.blender.org/blender/blender> plus the patch steps in this
repo's workflow file. See <https://www.blender.org/about/license/> for license details.

**"Blender" and the Blender logo are trademarks of the Blender Foundation.** This project is
unofficial and not affiliated with, endorsed by, or supported by the Blender Foundation.

## Credits

- The Blender Foundation and Blender contributors
- Megabits Studio — original tutorial on compiling Blender for iPad
