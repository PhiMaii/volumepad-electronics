# VolumePad STM32 PCB

Custom STM32-based PCB for the VolumePad project.

This board is intended for a haptic rotary input device with BLDC motor feedback, magnetic angle sensing, RGB LEDs, USB-C, buttons, strain sensing, and optional display support.

## Project status

Work in progress.

The current active development branch is `v2-redesign`.

The old version is kept on `v1-old`.

## Repository structure

    .
    ├── pcb/                 KiCad project files
    ├── docs/                Generated documentation, ignored by Git
    ├── fabrication/         Generated manufacturing files, ignored by Git
    ├── scripts/             Helper scripts
    ├── config.kibot.yaml    KiBot output configuration
    └── .github/workflows/   GitHub Actions automation

## PCB features

Planned / included hardware:

- STM32F405RGT6 microcontroller
- USB-C power and USB FS device connection
- TMC6300 BLDC motor driver
- MT6701 magnetic angle sensor
- WS2812B / SK6812 addressable RGB LEDs
- HX711-based strain sensing
- SWD programming connector
- Optional SPI display connection
- 4-layer PCB stackup

## KiCad project

Open the KiCad project from:

    open pcb/volumepad-stm32-pcb.kicad_pro

Main project files:

    pcb/volumepad-stm32-pcb.kicad_pro
    pcb/volumepad-stm32-pcb.kicad_sch
    pcb/volumepad-stm32-pcb.kicad_pcb

## KiBot automation

This repo uses KiBot through GitHub Actions to automatically generate documentation and manufacturing files.

Generated outputs include:

- Schematic PDF
- Gerber files
- Drill files
- BOM
- Pick-and-place position files

The workflow runs on changes to the PCB project or KiBot configuration.

Generated files are uploaded as GitHub Actions artifacts and are not committed to the repository.

## Generated files

Local generated outputs may appear in:

    docs/
    fabrication/

These files are intentionally ignored by Git.

## Notes

This PCB is still under active development and should not be considered production-ready yet.
