# PLC Export Directory Structure

## Directories
- `current/` - Latest XEF exports from Control Expert
- `backup/` - Historical XEF exports (use date folders YYYY-MM-DD)

## Export Process
1. Export from Control Expert to `current` folder
2. Copy to `backup/YYYY-MM-DD/` for version history
3. Commit and push changes to GitHub