# Artemis to RPCS3 Patch Converter (Alpha)

A tool for converting Artemis `.ncl` cheat files into RPCS3 **1.2-compatible** YAML patch format.

> **Mission (2026):** Emulation knowledge belongs to everyone.

## ⚠️ Alpha Release Notice
This is an alpha release. Some features may change. Back up your data and report issues.

## Features

### Database Management
- Smart file indexing (duplicate detection)
- Parse metadata (serial, name, version) from filenames
- Bulk import (folders / Artemis repos)
- Extract individual cheats with author credits

### Converter Engine
- RPCS3 1.2 YAML output
- Supports regular codes + AoB (Array of Bytes) + special formats
- Optional PPU hash (works with or without it)
- Preserves metadata (game info, cheat names, author credits)

### File Management
- Browse by file or grouped by game
- Search by game name / serial / filename
- Save patches to a local library
- Export YAML files

### Game Support
- BLUS / BLES / NPUB / NPEB serials
- Multiple versions per game

## Installation

### Prerequisites
- Python 3.7+
- Git

### Run
```bash
git clone https://github.com/chidreams/Artemis-to-RPCS3-Patch-Converter.git
cd Artemis-to-RPCS3-Patch-Converter
python artemis_converter.py
Usage Guide

Import

Quick Import NCL (single files)

Batch Import (folders)

Import Artemis Repo (existing Artemis databases)

Browse

Toggle: “Show Files” vs “Show by Game”

Use search box to filter

Convert

Select cheats → Add Selected Cheats

Fill Serial / Name / Version

PPU Hash optional (placeholder used if blank)

Convert → generate YAML

Save / Export

Save YAML File (export)

Save to Database (library)

Browse saved patches in “My Patches”

PPU-0000000000000000000000000000000000000000:
  "Patch Name":
    Games:
      "Game Name":
        BLUS12345: ["01.00"]
    Author: "NCL Converter"
    Notes: "Converted from Artemis NCL format"
    Patch Version: "1.2"
    Patch:
      - [ be32, 0xADDRESS, 0xVALUE ]

Project Structure
Artemis-to-RPCS3-Patch-Converter/
├─ artemis_converter.py
├─ README.md
└─ LICENSE

Known Issues (Alpha)

Some edge-case NCL files may not parse

Large repos may take time to index

UI optimization ongoing

License

