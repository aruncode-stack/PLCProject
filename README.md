# PLC Project Version Control

## Directory Structure
- `src/`
  - `main/original/`
    - `STU/` - Control Expert project files
    - `XDB/` - Database files
  - `lib/` - Reusable function blocks
- `exports/`
  - `current/` - Latest XEF exports
  - `backup/` - Dated backups (YYYY-MM-DD)
- `docs/`
  - `procedures/` - Export procedures
  - `specifications/` - Project specs
  - `standards/` - Coding standards
- `.github/workflows/` - CI/CD configurations

## File Placement Guide
1. Control Expert Files:
   - Place `.STU` files in: `src/main/original/STU/`
   - Place `.XDB` files in: `src/main/original/XDB/`
   - Export `.XEF` files to: `exports/current/`

## Version Control Steps
1. Export project from Control Expert as `.XEF`
2. Save to `exports/current/`
3. Create dated backup in `exports/backup/YYYY-MM-DD/`
4. Commit and push changes

## Important Notes
- Binary files (`.STU`, `.XDB`) are ignored by Git
- Only `.XEF` files in `exports/` are tracked
- Use meaningful commit messages