# 🌐 Cheprkach Browser

> **Custom WPF Web Browser** - Feature-rich Windows desktop browser with WebView2, built-in ad blocking, extensions, and cloud sync.

---

## 📋 Overview

Cheprkach is a custom Windows desktop browser built with WPF and Microsoft WebView2. It provides a modern browsing experience with features like tab management, bookmarks, downloads, ad blocking, extensions support, and cloud synchronization.

---

## 🎯 Features

- 🌐 **WebView2 Engine** - Chromium-based rendering via Microsoft Edge WebView2
- 📑 **Tab Management** - Multi-tab browsing with pinning and grouping
- 🔖 **Bookmarks** - Save and organize favorite sites
- 📥 **Download Manager** - Built-in download tracking and progress
- 🚫 **Ad Blocking** - Basic ad and tracker blocking
- 🧩 **Extensions** - Extension system with permission controls
- 🌙 **Dark Theme** - Toggle between light and dark modes
- ☁️ **Cloud Sync** - Synchronize data across devices
- 📱 **Session Restore** - Save and restore browsing sessions
- 📜 **History** - Browsing history with search

---

## 📁 Project Structure

| File | Description |
|------|-------------|
| `Program.cs` | Main browser implementation (49 KB) |
| `App.xaml` | Application resources |
| `Browser.csproj` | Project file |
| `Resources/` | Icons and resources |

---

## 🚀 Building & Running

### Requirements
- .NET 6.0 or later
- WebView2 Runtime (included with Windows 11, installable on Windows 10)
- Visual Studio 2022 or VS Code

### Build
```bash
dotnet build Browser.csproj
dotnet run
```

### Publish
```bash
dotnet publish -c Release -r win-x64 --self-contained
```

---

## ⚙️ Features in Detail

### Navigation
- URL bar with search integration
- Back/Forward/Refresh controls
- Home button (customizable homepage)

### Tab Features
- Create/Close tabs
- Pin important tabs
- Group related tabs
- Session persistence

### Bookmarks
- JSON-based storage
- Quick access from toolbar
- Import/Export capability

### Downloads
- Progress tracking with progress bar
- Download history
- Default download location

### Ad Blocking
- Block list for common ad domains
- Configurable blocking rules

### Extensions
- Permission-based system
- JavaScript injection support
- Extension management UI

### Cloud Sync
- JSON-based cloud storage
- Cross-device synchronization
- Automatic sync on changes

---

## 📝 Data Files

| File | Purpose |
|------|---------|
| `bookmarks.json` | Saved bookmarks |
| `session.json` | Tab session data |
| `cloud_sync.json` | Cloud synchronization data |
| `history.json` | Browsing history |

---

## 🎨 Customization

### Change Homepage
```csharp
homePage = "https://your-preferred-site.com";
```

### Modify Block List
```csharp
adBlockList.Add("new-ad-domain.com");
```

### Theme Toggle
- Built-in dark/light mode switch
- Persists across sessions

---

## 🛡️ Security

- WebView2 sandboxing
- Extension permission system
- No external credential storage
- Local data encryption potential

---

## 📝 Requirements

- Windows 10 1803+ or Windows 11
- WebView2 Runtime
- .NET 6.0 Runtime (if not self-contained)

---

## 📜 License & Disclaimer
---

## Comprehensive legal disclaimer

This project is intended for authorized defensive, administrative, research, or educational use only.

- Use only on systems, networks, and environments where you have explicit permission.
- Misuse may violate law, contracts, policy, or acceptable-use terms.
- Running security, hardening, monitoring, or response tooling can impact stability and may disrupt legitimate software.
- Validate all changes in a test environment before production use.
- This project is provided "AS IS", without warranties of any kind, including merchantability, fitness for a particular purpose, and non-infringement.
- Authors and contributors are not liable for direct or indirect damages, data loss, downtime, business interruption, legal exposure, or compliance impact.
- You are solely responsible for lawful operation, configuration choices, and compliance obligations in your jurisdiction.

---

<p align="center">
  <sub>Built with care by <strong>Gorstak</strong></sub>
</p>