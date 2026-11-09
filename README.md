# MPPS V18 — Drivers & Software

This repository contains the driver package and accompanying software for the **MPPS V18** car programming (ECU tuning/flashing) dongle.

> ## ⚠️ Disclaimer
>
> I do **not** own, create, or modify any of the files in this repository.
> All files are provided **as-is**, exactly as they were obtained.
> Download and use them **at your own risk**.
>
> No warranty is given, express or implied. The repository owner accepts no
> responsibility or liability for any damage, loss, or issues — including but
> not limited to damage to your vehicle, ECU, computer, or data — that may
> result from downloading or using these files. Make sure you understand what
> you are installing and accept the inherent risks of using third-party
> drivers and ECU programming tools.

## Contents

| Path | Description |
|------|-------------|
| `Mpps.exe` | Main MPPS V18 application |
| `MultiBoot.exe` | Multi-boot utility |
| `Tricore Boot.exe` | TriCore boot utility |
| `Device Driver/` | Dongle drivers — 32-bit & 64-bit installers plus AMT (AmtFlash) and FTDI packages for x86/amd64 |
| `Drives/` | Vehicle/ECU protocol driver files (`.Drv`) |
| `Check/` | Verification/checksum plug-ins (`Check###.dll`) |
| `Database/` | Software database file (`DataBase.Ini`) |
| `DtcCodes/` | Diagnostic trouble code definitions (`DDE5.Ini`, `Generic.Ini`) |
| `Language/` | Interface language files (38 languages) |
| `Mpps.Cfg`, `Tricore.Cfg` | Application configuration files |
| `Summary.Dat` | Session summary/history file |
| `*.Key` (`41363130.Key`, `Mpps.key`, `MultiBoot.Key`, `TPBoot.Key`) | Key/license files |
| `MPPS.gif` | Logo/image asset |

## Drivers

The `Device Driver/` folder contains installers and driver packages for both
32-bit and 64-bit Windows:

- `32 Bit Driver Installer.exe` / `64 Bit Driver Installer.exe`
- `AMT/` — AmtFlash driver package (`AmtFlash.sys`, `AmtFlash.inf`, `amtflash.cat`, plus `amd64`/`i386` subfolders)
- `FTDI/` — FTDI USB-to-serial driver package (`ftdibus.sys`, `ftd2xx.dll`, `ftd2xx.lib`, etc., for `amd64`/`i386` and `Static` linking)

## Usage

1. Install the appropriate driver for your system (32-bit or 64-bit) from the
   `Device Driver/` folder.
2. Connect the MPPS V18 dongle to a USB port and let Windows detect it.
3. Run `Mpps.exe` and select your vehicle/ECU.

## Notes

- Intended for **Windows** systems.
- Antivirus programs may flag ECU programming tools and unsigned drivers —
  this is common with this type of software, but proceed only if you trust the
  source.
- All files are distributed unmodified and without any support or warranty.

