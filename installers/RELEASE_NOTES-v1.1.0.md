# Smart Task Assistant v1.1.0

Full Windows installer (no admin). Installs to %LOCALAPPDATA%\Programs\SmartTaskAssistant.

## What's included

- Next.js production standalone server
- Portable Node.js runtime
- SmartTaskAssistant.exe launcher (Chrome app window, AppUserModelID Kiss.SmartTaskAssistant)
- Start Menu + Desktop shortcuts
- HKCU uninstall entry (no admin)

## Install

1. Download SmartTaskAssistant-Setup.exe
2. Double-click and confirm
3. Launch from Desktop / Start Menu

## Requirements

- Windows 10/11
- Google Chrome

## Google OAuth (optional)

Create .env.local in the install folder with GOOGLE_CLIENT_ID / GOOGLE_CLIENT_SECRET.
Redirect URI: http://localhost:3000/api/auth/google/callback

## Uninstall

Settings > Apps, or run Uninstall.exe /uninstall in the install folder.