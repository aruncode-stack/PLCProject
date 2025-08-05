# PLC Project Version Control

## Project Structure
- `src/`
  - `main/original/`
    - `STU/` - Control Expert project files
    - `XDB/` - Database files
    - `XEF/` - Binary export files
- `exports/`
  - `current/` - Latest XEF exports
  - `backup/` - Dated backups (YYYY-MM-DD)
- `docs/`
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