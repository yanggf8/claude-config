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