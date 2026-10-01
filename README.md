# XENEON EDGE Tuner Console

XENEON EDGE Tuner Console is an experimental Windows utility for discovering
connected CORSAIR XENEON EDGE displays and adjusting their display settings
over USB.

## What the App Does

The application provides controls for:

- OSD navigation, orientation, and automatic rotation.
- Brightness, contrast, backlight, and RGB color levels.
- Identifying and factory-resetting a selected XENEON EDGE display.
- Reading, saving, and applying display-setting profiles.
- Synchronizing settings across multiple connected XENEON EDGE displays.
- Choosing from persistent VS Code-inspired, CORSAIR Labs, Sensor Lime, and
  Teams Dark interface themes.
- Keeping a correlated Windows display orientation aligned with the physical
  display, with a confirmation countdown and automatic rollback protection.
- Confirming slider adjustments within 15 seconds, with automatic restoration
  of the previous display values if the countdown expires.

## Requirements

- A 64-bit Windows PC.
- A CORSAIR XENEON EDGE connected to the PC by USB and configured as an active
  Windows display.

The executable is self-contained; no installer or Python environment is
required.

## How to Use

1. Download the executable from the
   [latest GitHub Release](https://github.com/Corsair-Labs/XENEON-EDGE-Tuner-Console/releases/latest).
2. Place it in a writable folder. The application creates and updates
   `xe_profiles.json` beside the executable.
3. Connect the XENEON EDGE to the PC by USB and connect it as a Windows display.
4. Run the executable. The application scans for connected displays at startup.
5. Select a display from the **Xeneon** list. Use **Refresh** if a newly connected
   display does not appear, and **Identify** to confirm which display is selected.
6. Use the OSD, orientation, image-level, and color controls to tune the selected
   display.
7. Select **Show Profiles** to create, edit, read, save, or write reusable
   profiles. When multiple displays are connected, **Sync all connected
   displays** applies the selected display's settings to the others.
8. After a profile write, synchronized write, or slider adjustment, verify the
   result and select the corresponding **Keep** button before the countdown
   expires. Otherwise, the application restores the previous settings.

Because this executable is not digitally signed, Windows may show a security
warning. Only run software downloaded from a source you trust.

## Download Verification

Version: `0.13.13`

[Download Xeneon Edge Tuner Console v0.13.13](https://github.com/Corsair-Labs/XENEON-EDGE-Tuner-Console/releases/download/v0.13.13/Xeneon_Edge_Tuner_Console_v0.13.13.exe)

SHA-256:

```text
B8D04F42C65AA253D4F554B4C755BEDB394C44274D9A36ACCB0E84149D37F76B
```

## Disclaimer and License

This is experimental software, not a supported CORSAIR product. Review the
[DISCLAIMER NOTICE](DISCLAIMER%20NOTICE) and [LICENSE](LICENSE) before using or
redistributing it. The project uses the standard MIT License, which permits
commercial and non-commercial use, copying, modification, distribution,
sublicensing, and sale as long as the copyright and permission notices are
retained.

The license applies to the software, not to CORSAIR trademarks, product names,
logos, branding, or any claim of endorsement. The software is provided as-is,
without warranty or support.
