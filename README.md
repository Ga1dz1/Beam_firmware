
# Xreal Beam Firmware: Unofficial Update & Recovery Tools

**This repository provides resources for advanced users to update and recover their Xreal Beam devices. Proceed with caution as improper flashing can damage your device.**

## Contents

* **Full OTA Update Package:** Designed for flashing via sideload in recovery mode.
* **Fastboot Images:** Individual images for flashing specific partitions using Fastboot commands.

## Benefits

* **Flexibility:** Update your device outside of official channels.
* **Troubleshooting:** Recover from issues that may not be covered by standard support.
* **Customization:** Explore the potential for modifying your Beam's software (at your own risk).

## Instructions

### OTA Update (Sideload)

1. Connect your Beam to your computer via USB.
2. Download the latest OTA package (`update.zip`) from the releases section.
3. Boot your Beam into recovery mode.
4. Select "Apply update from ADB."
5. Run the following command, replacing `<file_name>` with the actual file:

   ```bash
   adb sideload <file_name>.zip
   ```

### Fastboot Flashing

1. Connect your Beam to your computer via USB.
2. Download the Fastboot image set (`.img` files) from the releases section.
3. Boot your Beam into Fastboot mode.
4. Flash each image using the appropriate partition name:

   ```bash
   fastboot flash <partition_name> <file_name>.img
   ```
   (Common partition names: `boot`, `system`, `vendor`, etc.)

## Important Notes

* **Backup:**  Before proceeding, back up all important data as flashing can erase your device.
* **Battery:** Ensure your Beam is sufficiently charged to avoid interruptions.
* **Research:** Familiarize yourself with Fastboot and recovery procedures before starting.

## Disclaimer

This is an unofficial project. We are not affiliated with Xreal and do not provide any warranty or guarantee. Use these tools at your own risk.
