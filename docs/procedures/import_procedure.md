# PLC Import Procedure

## Control Expert Import Steps
1. Open Control Expert
2. Create new project or open existing
3. Select Project → Import
4. Choose Text file:
   - Navigate to `exports/current/`
   - Select latest `ProjectName_YYYYMMDD.txt`
   - Verify UTF-8 encoding

## Validation Steps
1. Check Project Structure
   - Verify all sections imported
   - Check for missing FBDs
   - Validate data types

2. Test Imported Code
   - Use simulation mode if available
   - Check for compilation errors
   - Verify FB connections

## Recovery Steps (if needed)
1. If import fails:
   - Check `exports/backup/` for previous version
   - Document import errors
   - Revert to last known good backup

## Version Control Notes
1. Create recovery branch:
   ```powershell
   git checkout -b recovery/YYYY-MM-DD
   ```
2. Document import issues:
   ```powershell
   git commit -m "Import recovery: [Description of issues]"
   ```

## Important Notes
- Always backup current project before import
- Test in simulation before deploying
- Document any modifications needed after import
- Keep original export file for reference