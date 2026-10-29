# NGPT OS

NGPT OS is a Windows-inspired desktop workspace that runs in a web browser. This is an early preview, not a native operating system.

## Deploy to Vercel
1. Import this repository into Vercel.
2. Select **Other** as the framework preset if asked.
3. Leave the build command empty.
4. Use `.` as the output directory if Vercel asks for one.
5. Deploy.

No API keys or build step are required for the preview.

## Included
- Windows-inspired desktop, Start menu, taskbar, draggable/maximizable windows
- Browser preview with DuckDuckGo search and open-in-new-tab fallback
- File Explorer with local notes and uploaded files
- EXE Folder for storing/downloading Windows installer files (does not execute them)
- File Locker using browser Web Crypto AES-GCM encryption and a password-derived key
- App Store, Settings, Calculator, Calendar, Clock, Paint, Notepad, Terminal preview, System Info
- Wallpaper, accent colour, light/dark theme, glass effects, taskbar alignment, UI scale, local profile name
- Local settings export/import

## Important browser limits
- Websites may block iframe previews. Use the external-tab button in Browser for those sites.
- Browser file access is permission-based; a website cannot silently browse all your PC folders. Files you import are stored in this browser's IndexedDB.
- Local profile name is not online authentication. A real Supervisor account with secure login/roles and cross-device sync requires an authentication/database service.
- File Locker encrypts file contents before saving them locally. Keep a backup and remember the password; forgotten passwords cannot recover the vault. Browser storage can be cleared by the browser or device, so this preview is not a substitute for a backed-up secure vault.
- Browsers cannot run Windows .exe programs. The EXE Folder is for storage/download only.
- Native Windows/Linux versions need a separate desktop wrapper/build and additional testing.

## Local data
Settings, notes, browser history, and vault data are stored locally in the browser. They do not automatically sync between devices.
