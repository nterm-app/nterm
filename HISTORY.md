# Release History

## v0.0.7 (2025-12-28)

### Features

#### Agents Support
- Add and manage AI agents from web dashboard
- Sync agents to terminal via `nterm agents sync`
- Create custom agents with specific configurations
- Agents available across all terminal sessions
- Seamless integration with existing terminal workflows

---

## v0.0.5 (2025-12-05)

### Features

#### Terminal Settings Sync
- Customize terminal appearance from web dashboard (background color, text color, font size, font family, cursor style, cursor blink)
- Real-time sync to terminal app via 5-second polling
- Settings automatically reset to defaults when session is revoked
- User profile hidden when session is deleted from dashboard

#### Environment Types
- Support for multiple environment types per project (development, staging, production, etc.)
- `nterm env sync` - Sync development environment (default)
- `nterm env sync <type>` - Sync specific environment type (e.g., `nterm env sync staging`)
- Manage environment types from web dashboard

### Web Dashboard

#### Terminal Detail Page
- New tab-based layout (Information / Settings)
- Terminal settings tab with live preview
- Color pickers for background and text colors
- Font size slider, font family selector
- Cursor style and blink options

#### Environment Detail Page
- Add, edit, and delete environment types
- Separate variables per environment type
- Sync hint showing correct CLI command for each type

### Downloads

| File | Architecture |
|------|--------------|
| `nterm-0.0.5-arm64.dmg` | Apple Silicon (M1/M2/M3) |
| `nterm-0.0.5.dmg` | Intel (x64) |

---

## v0.0.4 (2025-12-03)

### Features

#### Multiline Input
- Add Shift+Enter support for multiline input in apps like Claude CLI

#### Link Opening
- Add Cmd+Click to open terminal links in default browser

#### Drag & Drop
- Add drag & drop support to paste file paths into terminal

#### Git Dirty State
- Add red `*` indicator next to branch name when there are uncommitted changes

### Bug Fixes

#### Keyboard
- Fix Option+Q to type `@` character (macOptionIsMeta: false)

### Downloads

| File | Architecture |
|------|--------------|
| `nterm-0.0.4-arm64.dmg` | Apple Silicon (M1/M2/M3) |
| `nterm-0.0.4.dmg` | Intel (x64) |

---

## v0.0.3 (2024-12-03)

### Bug Fixes

#### PATH Environment
- Added standard system paths to PATH environment
- Fixed issue where commands like `claude`, `brew`, etc. were not found
- Electron apps launched from Finder now include `/usr/local/bin` and `/opt/homebrew/bin`

### Downloads

| File | Architecture |
|------|--------------|
| `nterm-0.0.3-arm64.dmg` | Apple Silicon (M1/M2/M3) |
| `nterm-0.0.3.dmg` | Intel (x64) |

---

## v0.0.2 (2024-12-03)

### Features

#### User Profile in Titlebar
- Display logged-in user's avatar, name, and email in titlebar
- Auto-updates profile on login/logout (no restart required)
- Click profile to open dashboard in browser
- Fallback to initials when avatar is unavailable

#### Account Management
- `nterm account` - Login to nterm account via browser authentication
- `nterm account logout` - Logout from account
- `nterm account status` - Check current login status

#### Environment Sync
- `nterm env sync` - Apply environment variables from cloud
- `nterm env unsync` - Reset to default LTS and clear env variables
- Automatic Node.js version installation during sync

### Improvements

#### UI/UX
- Redesigned titlebar with unified height for version badge and profile
- Improved styling for Node.js version display
- Better visual consistency across titlebar elements

#### Backend (nterm-api)
- File-based avatar upload system (replaces base64 storage)
- Static file serving for uploaded avatars
- Improved avatar URL handling

#### Frontend (nterm-landing)
- Added "Go to Terminals" button on device authorization success page
- Fixed avatar URL transformation in API methods

### Downloads

| File | Architecture |
|------|--------------|
| `nterm-0.0.2-arm64.dmg` | Apple Silicon (M1/M2/M3) |
| `nterm-0.0.2.dmg` | Intel (x64) |

---

## v0.0.1 (2024-12-02)

**Initial Release**

### Features

#### Terminal
- Fast, GPU-accelerated terminal powered by xterm.js
- Native macOS look with hidden title bar
- 256-color and true color support
- Clickable URLs
- Search functionality (`Cmd+F`)
- Zoom in/out (`Cmd++` / `Cmd+-`)

#### Split Panes
- Split horizontally (`Cmd+D`)
- Split vertically (`Cmd+Shift+D`)
- Navigate between panes (`Cmd+]` / `Cmd+[`)
- Resizable dividers
- Per-pane Node.js version support

#### Node.js Version Manager
- `nterm node list` - View installed versions
- `nterm node install <version>` - Install any version
- `nterm node use <version>` - Switch versions
- `nterm node remove <version>` - Remove versions
- Support for `lts` and `latest` keywords
- Auto-install missing versions

#### Auto Version Switching
- `.nterm` file support for project-specific Node.js versions
- Automatic version switching when entering directories

#### Shell Integration
- Custom prompt with git branch display
- Separate history file (`~/.nterm/history`)
- User config at `~/.nterm/config`
- Pre-configured aliases

### Downloads

| File | Architecture |
|------|--------------|
| `nterm-0.0.1-arm64.dmg` | Apple Silicon (M1/M2/M3) |
| `nterm-0.0.1.dmg` | Intel (x64) |

### System Requirements
- macOS 10.15 (Catalina) or later
