# Release History

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
