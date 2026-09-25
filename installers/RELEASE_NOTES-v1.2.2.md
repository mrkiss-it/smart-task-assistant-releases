# Smart Task Assistant v1.2.2

Vietnamese UI diacritics (dấu), Start Menu / Pin-to-Start polish, Setup branding fix.

## Highlights
- All Vietnamese installer + app UI strings use proper diacritics (UTF-8)
- Single Start Menu entry: **Smart Task Assistant** → installed `SmartTaskAssistant.exe` (not Chrome, not Setup)
- Setup.exe branded as **Smart Task Assistant Setup** (does not register as the product app)
- Proper multi-size `.ico` on launcher + shortcuts; AppUserModelID `Kiss.SmartTaskAssistant` for Pin to Start
- Setup / Uninstall version **1.2.2**

## Install
1. Download `SmartTaskAssistant-Setup.exe`
2. Run the wizard (Welcome → Options → Progress → Finish)
3. Options: Desktop shortcut (default on), Start with Windows (default off), Launch when finished (default on)
4. Quiet: `SmartTaskAssistant-Setup.exe /quiet`

Upgrades preserve `data\`, `ChromeAppProfile\`, `logs\`, and `.env.local`.

## Requirements
- Windows 10/11
- Google Chrome (app window)

## Google OAuth (optional)
Create `.env.local` in the install folder with `GOOGLE_CLIENT_ID` / `GOOGLE_CLIENT_SECRET`.
Redirect URI: `http://localhost:3000/api/auth/google/callback`
See `.env.example` shipped in the install folder. **No Google secrets are baked into the installer.**

## Uninstall
Settings → Apps, or run `Uninstall.exe /uninstall` (`/quiet` supported).