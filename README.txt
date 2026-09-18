Police Duty Rotation V4

This package is based on the existing FINAL-PRODUCTION-V3 design and preserves its visual branding.
V4 additions include:
- Station-wise PI/PSI/ASI/HC/PC requirement table
- Event/date/time/station/route/point deployment
- Automatic name allocation with rank, availability, rotation and time-conflict checks
- Cross-station reallocation at different times
- Local app lock with PBKDF2 password verification and auto-lock
- Offline-first Electron shell with blocked unknown external HTTP requests
- Gujarati Unicode/joining-character support retained through UTF-8 and Gujarati font fallbacks
- Existing backup, error monitoring and production hardening retained

Security note: no software can honestly guarantee zero compromise. This build minimizes exposure by keeping data local/offline, requiring a local lock, protecting backups separately, and preventing the desktop shell from silently making unknown external HTTP requests. Sensitive CM/PM/VIP data should still be handled according to departmental cyber-security policy.

Build:
- Windows: npm install && npm run dist
- Android: npx cap add android && npx cap sync android && cd android && ./gradlew assembleDebug
