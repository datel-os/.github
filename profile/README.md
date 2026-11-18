<img src="logo.svg" width="96" align="right" alt="Datel OS">

# Datel OS

Open firmware for the Creality K1 3D printer, built from source with Yocto: Linux 6.18, zklippy (Kalico's Klipper host as one Zig binary) with open firmware for all three MCUs, Moonraker, Mainsail, camera streaming, hardware-encoded timelapse and Twitch live streaming. The stock bootloader stays in place, and the printer's second system slot always holds a way back.

It is a pre-release for developers: it runs on its author's printer, everything is verified on that one machine, and the display does not work yet. Read [what works](https://github.com/datel-os/datel-os#what-works) and the [limitations](https://github.com/datel-os/datel-os#limitations) before you install anything.

## Where to start

| | |
|---|---|
| [Releases](https://github.com/datel-os/datel-os/releases) | The kernel, the system image and the checksums of every version |
| [Install](https://github.com/datel-os/datel-os/blob/main/docs/INSTALL.md) | Backup, writing the unused slot, the trial boot, going back to stock, recovery |
| [Documentation](https://github.com/datel-os/datel-os#documentation) | The host and the MCU firmware, camera, Twitch, diagnostics, hardware, how a release is made |

## Repositories

| Repository | What it holds |
|---|---|
| [datel-os](https://github.com/datel-os/datel-os) | The releases, and the Yocto layer, tools and documents as they were at each release |
| [k1-linux](https://github.com/datel-os/k1-linux) | The kernel: kernel.org 6.18 plus the support for the K1's Ingenic X2000, every change through a pull request |
| [k1-kalico-firmware](https://github.com/datel-os/k1-kalico-firmware) | Kalico's MCU firmware for the K1's three GD32 boards |

Day-to-day work on the layer happens in a private repository and reaches `datel-os` with its history at every release. zklippy is developed in a private repository too; it is GPLv3, and each release carries the source of the commit it was built from.

## The name

*Datel* is Czech for woodpecker. The bird in the logo is one.
