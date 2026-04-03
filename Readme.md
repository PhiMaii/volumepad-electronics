# VolumePad Electronics

Hardware design repository for VolumePad PCBs and board-level assets.

This repository is a submodule of the main VolumePad umbrella repo and contains KiCad projects for the hardware platform.

## Role In The Full Stack

In the full VolumePad architecture:
- electronics defines the physical boards and connectivity
- firmware targets the hardware designed here
- desktop and plugin software assume the hardware/protocol behavior

## Project Layout

- `mainboard/`: main PCB design files
- `touch_board/`: touch/auxiliary board design files
- `usb_hub_board/`: USB hub board design files
- `panel/`: panel-related assets/placeholders

## Working With The Designs

Open the `.kicad_pro` files in KiCad for schematic/PCB editing and fabrication export workflows.

## Documentation Policy

Global architecture/protocol/layout docs are maintained only in:
`D:\Daten\Programmieren\volumepad\docs`

Use this submodule docs area only for electronics-specific notes that do not redefine global contracts.
