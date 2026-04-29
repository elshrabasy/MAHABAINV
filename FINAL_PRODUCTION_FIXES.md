# Final Production Fixes

Applied in this release:

- Added `asarUnpack` for Realm native `.node` bindings.
- Exported `closeRealm()` and call it on application shutdown.
- Hardened `restoreBackup()` so Realm reopens even if restore fails.
- Removed visible demo credentials from the login UI.
- Removed quick-login buttons that displayed login shortcuts.
- Removed `unsafe-eval` from Content Security Policy.
- Fixed `window.d.ts` API optionality.
- Fixed browser/local fallback report export functions.
- Kept GitHub Actions output in `release/`.

Test flow:
1. Run GitHub Actions workflow.
2. Download the artifact.
3. Test `release/win-unpacked/Mahabat Alfan ERP.exe` first.
4. Install the generated setup after the unpacked app opens correctly.
