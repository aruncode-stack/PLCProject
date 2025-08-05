# PLC Project Version Control

## Project Structure
- `src/` - FBD source files
  - `main/` - Main program blocks
  - `lib/` - Reusable function blocks
- `exports/` - Exported text versions
  - `backup/` - Dated backups
  - `current/` - Latest exports
- `docs/` - Documentation
  - `procedures/` - Export procedures
  - `standards/` - Coding standards

## Version Control Guidelines
1. Export FBD code as text before committing
2. Include descriptive commit messages
3. Document major changes in docs folder
4. Use feature branches for development
5. Tag production releases

## Export Procedure
1. Open Control Expert
2. Export FBD as text
3. Save to `exports/current` directory
4. Backup to `exports/backup/YYYY-MM-DD/`

## Tools Used
- Control Expert (Unity Pro)
- Git version control
- VS Code editor