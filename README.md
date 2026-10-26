# Xiegu-X6200---Lab599-Style-Modification
Xiegu X6200 - Lab599 Style  Modification
OpenX6X00 X6200 — Lab599 Monochrome Edition
Based on OpenX6X00 v0.3.4

FILE
Lab599-X6200-v0.3.4.img
Size: 481 MiB, uncompressed
Radio: Xiegu X6200

OVERVIEW
This custom SD-card image provides a monochrome interface inspired by the Lab599 TX-500.

It uses the same visual preset as the previous X6100 version:
- Pale LCD background and black lettering
- Large frequency digits
- Square controls
- Monochrome menus and meters
- Filled spectrum and greyscale waterfall

Normal mode and the existing walkie-talkie mode remain available.

INSTALLATION
1. Download Lab599-X6200-v0.3.4.img.
2. Insert a separate microSD card into your computer.
3. Open your usual disk-image writer.
4. Select the .img file as the source.
5. Carefully select the microSD card as the destination.
6. Write the image and allow verification to finish.
   WARNING: This erases the selected card.
7. Safely eject the card.
8. With the X6200 powered off, insert the card.
9. Boot using the original OpenX6X00 X6200 SD-card procedure.

The Lab599-Mono theme is selected automatically on first boot.

NORMAL AND WALKIE-TALKIE MODES
Use the firmware’s existing Walkie Talkie setting to switch modes.

The modification changes the display preset. It does not add frequency coverage, radio modes or transmit capabilities.

SETTINGS
The display preset applies once. Later display changes are retained.

When an existing DATA partition is available, settings are backed up before the preset is applied:

/mnt/params.before-lab599.db

Only display-related values are changed. Saved walkie-mode selection, channels, tuning and power settings are retained.

To change the appearance, select another theme in Settings > Display.

CARD COMPATIBILITY
Unused filesystem space was reduced to fit the download limit. All firmware files were preserved.

The smaller root partition changes where a fresh card creates its DATA partition. DATA from a previous larger image is not automatically migrated.

Use a separate card and back up existing settings and files before rewriting any previously used card.

APPEARANCE
This is a Lab599-inspired adaptation, not a pixel-identical TX-500 interface.

Fonts, meter placement and the portrait walkie-talkie layout follow OpenX6X00.

Startup artwork, the web interface and picture content such as SSTV retain their original appearance.

VERIFICATION
- All 128 interface theme colour roles are monochrome.
- The v0.3.4 theme parser accepted the theme.
- Settings application, backup and one-time behavior were tested.
- SQLite and filesystem integrity checks passed.
- Original firmware files and symbolic links were preserved.
- The original X6200 kernel, bootloader, programs and radio-control library remain unchanged.

This image has not been booted or tested on a physical X6200. Screen appearance, controls and RX/TX operation still require an on-radio check.

SHA-256
72fb2f414762c4a7ca18bf1d2796605e045f7e4bef039d2620351fc98f15663d
