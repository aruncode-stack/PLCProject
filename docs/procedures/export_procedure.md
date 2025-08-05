# PLC Export Procedure

## Control Expert Export Steps
1. Open project in Control Expert
2. Select Project → Export
3. Choose Text format
4. Save to: `exports/current/`
5. Copy to: `exports/backup/YYYY-MM-DD/`

## Version Control Steps
1. Stage changes: `git add .`
2. Commit with message: `git commit -m "Export YYYY-MM-DD"`
3. Push to GitHub: `git push origin main`