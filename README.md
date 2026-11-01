# NOVEMBER

A local-first 30-day November challenge tracker built with React, TypeScript and Vite.

## Privacy and storage

NOVEMBER does not require an account and does not send check-ins to an application server. The display name and daily records are stored in the browser's localStorage on the current device. Anyone with access to the same browser profile may be able to view that local data; clearing browser storage may erase it.

The Profile page supports ordinary PDF, CSV and JSON exports, plus an encrypted backup file. Encrypted backups use PBKDF2-SHA-256 (310,000 iterations) to derive an AES-256-GCM key from a user-chosen passphrase, with a fresh random salt and IV for each backup. The passphrase is not transmitted. Restoring requires the same passphrase and replaces the local progress after confirmation. If the passphrase is lost, the backup cannot be recovered.

Use the deployed site over HTTPS for Web Crypto support. This encryption applies to exported backup files; it does not encrypt localStorage itself.

## Development

```bash
npm install
npm run dev
```

## Production build

```bash
npm run build
```
