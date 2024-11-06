# Editor Configurations

This repository contains configuration files for my code editors:

- Visual Studio Code
- Cursor

## Repository Structure

- `vscode-settings.json` - Visual Studio Code configuration
- `cursor-settings.json` - Cursor configuration
- `setup.sh` - Installation script for new machines

## Original File Locations

- Visual Studio Code: `~/Library/Application Support/Code/User/settings.json`
- Cursor: `~/Library/Application Support/Cursor/User/settings.json`

## Purpose

This repository is used for:

- Storing configuration backups
- Synchronizing settings between different computers
- Tracking configuration changes
- Easy restoration of previous settings versions

## How to Use

### Automatic Setup

1. Clone the repository
2. Make the setup script executable:

   ```bash
   chmod +x setup.sh
   ```

3. Run the setup script:

   ```bash
   ./setup.sh
   ```

### Manual Setup

If you prefer to set up manually:

1. Clone the repository
2. Create hard links to appropriate system locations:

   ```bash
   ln vscode-settings.json ~/Library/Application\ Support/Code/User/settings.json
   ln cursor-settings.json ~/Library/Application\ Support/Cursor/User/settings.json
   ```

3. All file changes will be automatically synchronized

## Notes

- The setup script will automatically backup any existing configurations
- Backup files will have `.backup` extension
- The script will create necessary directories if they don't exist
# vs-cursor-sync-
