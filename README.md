# Artemis to RPCS3 Patch Converter (Alpha Release)

![Python](https://img.shields.io/badge/python-3.7%2B-blue)
![Status](https://img.shields.io/badge/status-alpha-yellow)
![License](https://img.shields.io/badge/license-MIT-green)
![Platform](https://img.shields.io/badge/platform-windows%20%7C%20linux%20%7C%20macOS-lightgrey)

A powerful tool for converting Artemis NCL cheat files into RPCS3 1.2-compatible YAML patch format. This alpha release focuses on core functionality with more features coming soon.

## ⚠️ Alpha Release Notice
This is an **alpha release** - while functional, some features may be incomplete or undergo significant changes. Back up your data before use and report any issues you encounter.

## 🚀 Features

### 🗃️ **Database Management**
- **Smart File Indexing**: Automatically parse and organize NCL files with duplicate detection
- **Intelligent Parsing**: Extract game metadata (serials, names, versions) from filenames
- **Bulk Operations**: Import entire folders or Artemis repositories
- **Cheat Extraction**: Parse NCL content to separate individual cheat codes with author credits

### 🔄 **Converter Engine**
- **RPCS3 1.2 Compliance**: Generate properly formatted YAML patches
- **Multi-Format Support**: Regular codes, AoB (Array of Bytes), and special format codes
- **Optional PPU Hash**: Works with or without PPU hash for testing
- **Metadata Preservation**: Maintain game info, cheat names, and author credits

### 📂 **File Management**
- **Dual View Modes**: Browse by individual files or grouped by game
- **Real-time Search**: Filter by game name, serial, or filename
- **Cheat Library**: Save and organize converted patches
- **Export Options**: Save patches as YAML files for RPCS3

### 🎮 **Game Support**
- **Multi-Region**: BLUS, BLES, NPUB, NPEB serial formats
- **Version Handling**: Support for multiple game versions
- **Cheat Organization**: Group cheats by game and version

## 📦 Installation

### Prerequisites
- Python 3.7 or higher
- Git (for cloning repository)

🖥️ Usage Guide
1. Database Setup

    Click "Quick Import NCL" to add individual files

    Use "Batch Import" for entire folders

    "Import Artemis Repo" for existing Artemis databases

2. Browse Cheats

    Switch between "Show Files" and "Show by Game" views

    Use search box to filter results

    Double-click files to view details and cheats

3. Convert to RPCS3 Format

    Select cheats and click "Add Selected Cheats"

    Fill in game metadata (Serial, Name, Version)

    PPU Hash is optional (placeholder used if empty)

    Click "Convert" to generate YAML

4. Save & Export

    "Save YAML File" to export patch

    "Save to Database" for library storage

    Browse saved patches in "My Patches" tab   
🛠️ Technical Details
Database Schema
sql

games:        Game metadata and file information
cheats:       Individual cheat codes linked to games
user_patches: Saved RPCS3 patches
indexed_files: File tracking with hash verification

File Format Support

    Input: .ncl (Artemis cheat files)

    Output: .yaml (RPCS3 1.2 patch format)

    Database: SQLite with WAL mode for performance

YAML Output Format
yaml

PPU-0000000000000000000000000000000000000000:
  "Patch Name":
    Games:
      "Game Name":
        BLUS12345: [ "01.00" ]
    Author: NCL Converter
    Notes: Converted from Artemis NCL format
    Patch Version: 1.2
    Patch:
      - [ be32, 0xADDRESS, 0xVALUE ]

📁 Project Structure
text

artemis-converter/
├── artemis_converter.py    # Main application
├── artemis_converter.db    # Database (auto-created)
├── NCL_Files/              # Imported NCL storage
├── User_Patches/           # Exported patches
└── README.md               # This file

🔧 Configuration
Settings

Access via ⚙️ Settings button:

    Debug Mode: Enable detailed parsing output

    Context menu settings

    Display preferences

Keyboard Shortcuts

    Ctrl+C: Copy selected text

    Ctrl+V: Paste from clipboard

    Ctrl+A: Select all text

    Right-click: Context menu with copy/paste options

🐛 Known Issues (Alpha)

    Some edge-case NCL files may not parse correctly

    Large repositories may take time to index

    UI may need optimization for very large cheat collections

    Settings persistence between sessions is basic

