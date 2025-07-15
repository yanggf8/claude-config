## Troubleshooting

### TypeScript and Caching
- For empty ts files, try the cache clearing command first:
  ```
  # Clear all caches and restart fresh
  npm run clear-cache
  npm run dev:fresh

  # If that doesn't work, try a full rebuild
  npm run build
  ```

### Server Startup
- When starting server, always ask the developer to confirm or initiate the startup process

## Git Configuration

### File Syncing
- `.credentials.json` is gitignored to preserve local login across machines
- `statsig/` cache files are gitignored to prevent session conflicts and maintain analytics accuracy
- Only sync configuration files (CLAUDE.md, project configs, etc.) across machines

### Merging Strategy
- Use merge strategy for pulls: `git pull --no-rebase`
- For unrelated histories: `git pull --no-rebase --allow-unrelated-histories`

- update docs before commit

## Database Considerations
- No constraint in db, especially in document databases
- No constraint in db, especially in relational databases (RDB)