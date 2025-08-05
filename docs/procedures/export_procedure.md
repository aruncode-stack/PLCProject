# PLC Export Procedure

## Control Expert Export Steps
1. Open project in Control Expert
2. Select Project → Export
3. Choose Text format
   - Select "All Sections"
   - Enable "Include Comments"
   - Set Character Set to "UTF-8"
4. Save to: `exports/current/`
   - Use format: `ProjectName_YYYYMMDD.txt`
5. Copy to: `exports/backup/YYYY-MM-DD/`
   - Keep dated backups for rollback purposes

## Version Control Steps
1. Stage changes: `git add .`
2. Commit with message: `git commit -m "Export YYYY-MM-DD: [Brief description]"`
3. Push to GitHub: `git push origin main`

## Important Notes
- Always export before making major changes
- Include meaningful commit messages
- Verify exports are in text format
- Keep backup copies in `exports/backup/`
- Test imported files after export