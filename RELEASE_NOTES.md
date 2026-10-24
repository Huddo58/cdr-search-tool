# Release notes

## v1.1.0 — 24 October 2026

First stable public release with permanent Full Licence activation.

- Free Edition retains up to 30 days of call records.
- A$100 one-time Full Licence unlocks longer configurable retention for one installation.
- Full licences have no expiry and include future Call Records updates.
- Installation-bound RSA licence validation works offline and persists across restarts.
- Invalid activation attempts preserve an existing valid licence.
- Cleanup pauses if a stored licence needs attention, protecting existing records during recovery.
- Includes search, SFTP ingestion, historical import, CDR on Demand, reporting, exports,
  schedules, user roles, audit history, SMTP and storage policies.
- Includes the Node.js runtime and production dependencies in a portable Windows package.
- Core application JavaScript, including licensing, is obfuscated.

The developer has validated the download → purchase → licence delivery → activation
flow end to end. The experimental data-verification feature remains excluded.

### Package integrity

File: `CallRecords-v1.1.0-Windows.zip`  
Size: **46,186,479 bytes**  
SHA-256: `8682a3ce9fc63f0bb7b913f47d5ef82bd1cb0b0625fd7b512d543816de697f2b`

Back up and preserve the complete data folder during updates. See the
[user guide](https://scotthudson.com.au/projects/call-records/docs) before changing
an existing installation.
