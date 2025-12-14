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

### Quick Start
```bash
# Clone the repository
git clone https://github.com/Chidreams/artemis-converter.git
cd artemis-converter

# Run the application
python artemis_converter.py


