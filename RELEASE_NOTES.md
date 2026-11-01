# Release notes

## v1.2.0 - 1 November 2026

- Windows service with automatic startup and failure recovery, independent of the Manager, browser and signed-in user.
- Native Manager for installation/migration, start/stop/restart, updates, code rollback and diagnostics; configurable web port (default 3080).
- Existing database, call archives, installation identity, licence and encryption keys are preserved during managed updates. Code rollback preserves newer records.
- Licensing has its own sidebar page. Existing Free/Full terms are unchanged.
- Manual Data Gap Check: horizontal 24-hour daily timelines, clickable details, cluster and individual-manager activity.
- Separate filename evidence for sequence discontinuities, resets, failed/pending imports, duplicates and conflicting receipts; configurable verified node roles and thresholds.
- Checks are read-only and limited to a selected period of up to 31 days. Quiet intervals and sequence candidates do not certify missing records or completeness. No automatic repair or deletion.
- First-party application JavaScript is obfuscated and the runtime/dependencies are included.

The package is unsigned. Windows administrator approval is required for service installation; organisational software/signing rules still apply. Installer actions do not bypass firewall or endpoint policy.

Before updating, back up the complete data folder, extract the new package separately and close installed Manager windows. Use a maintenance window and verify your live CUCM feed after migration. See the user guide for supported layouts and rollback details.

File: `CallRecords-v1.2.0-Windows.zip`  
Size: **36,398,639 bytes**  
SHA-256: `caff9c2762268f5dbfd1420fdc0aebe840ac93cb3f1668322701072339934bb7`


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
