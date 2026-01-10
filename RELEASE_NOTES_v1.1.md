# ZenOptimize v1.1 - Release Notes

## 🎮 Enhanced Gaming Experience

### What's New

#### Major Features
1. **Windows Game Mode Integration**
   - Automatically enables Game Mode for optimal gaming resource allocation
   - Windows prioritizes game performance over background tasks

2. **Hardware-Accelerated GPU Scheduling (HAGS)**
   - Reduces GPU latency on supported hardware
   - Automatic Windows version detection (requires Build 19041+)
   - Smart restart prompting (only when newly enabled)
   - Graceful handling for unsupported GPUs

3. **Distraction-Free Gaming**
   - Disables Focus Assist to prevent interruptions
   - Suppresses Windows notifications during gameplay
   - Cleaner, more focused gaming sessions

4. **Xbox Services Optimization**
   - Disables non-essential Xbox services (XblAuthManager, XblGameSave)
   - **Preserves Xbox controller support**
   - Reduces background overhead

5. **Comprehensive Logging System**
   - Detailed log file (ZenOptimize.log) created alongside the executable
   - Timestamped entries for all operations
   - INFO/WARN/ERROR level logging
   - Perfect for troubleshooting and verifying changes

#### Improvements
- **Enhanced Administrator Elevation**
  - Works seamlessly with both .ps1 and compiled .exe (ps2exe)
  - No manual intervention required
  - Respects system UAC configuration

- **Smart HAGS Detection**
  - Only prompts for restart when HAGS is newly enabled
  - Skips restart prompt if HAGS was already enabled
  - Better user experience

- **Updated Backup System**
  - All v1.1 settings included in backup
  - Full restore capability for all new features

### Technical Details

#### New Registry Modifications
- `HKCU:\Software\Microsoft\GameBar` - Game Mode settings
- `HKLM:\SYSTEM\CurrentControlSet\Control\GraphicsDrivers` - HAGS configuration
- `HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\QuietHours` - Focus Assist
- `HKCU:\Software\Microsoft\Windows\CurrentVersion\Notifications\Settings` - Notifications
- `HKLM:\SYSTEM\CurrentControlSet\Services\XblAuthManager` - Xbox authentication service
- `HKLM:\SYSTEM\CurrentControlSet\Services\XblGameSave` - Xbox game save service

#### System Requirements
- Windows 10 Build 19041+ (for HAGS support)
- Administrator privileges (auto-elevated)
- Compatible GPU driver (for HAGS - automatically detected)

### How to Upgrade from v1.0
1. Download `ZenOptimize_v1.1.exe`
2. Run the executable
3. Choose "Apply Optimizations"
4. If HAGS is enabled, you'll be prompted to restart (recommended)

Your existing v1.0 settings will be preserved and extended with v1.1 features.

### Files Generated
- `ZenOptimizeBackup.json` - Full backup of all registry changes
- `ZenOptimize.log` - Detailed operation log with timestamps

### Restore Capability
All v1.1 changes are fully reversible:
1. Run ZenOptimize
2. Choose "Restore Defaults"
3. All settings return to their original values

### Known Behavior
- HAGS requires a system restart to take effect
- Xbox controller functionality is preserved despite service optimization
- Logging is silent-fail (won't interrupt operation if log file can't be written)

---

## Compilation Instructions (for distribution)

To compile the .ps1 to .exe using ps2exe:

```powershell
ps2exe -inputFile "ZenOptimize.ps1" -outputFile "ZenOptimize_v1.1.exe" -requireAdmin -iconFile "ZenOptimize.ico"
```

**Notes:**
- Do NOT use `-noConsole` parameter. The script requires an interactive console for the menu system and user prompts.
- The `-iconFile` parameter adds the ZenOptimize icon to the executable.

---

## Testing Checklist

- [x] Administrator auto-elevation (.ps1)
- [x] Administrator auto-elevation (.exe compiled with ps2exe)
- [x] HAGS detection and enablement
- [x] HAGS already-enabled detection (no restart prompt)
- [x] Game Mode enablement
- [x] Xbox services optimization
- [x] Focus Assist and notification suppression
- [x] Comprehensive logging
- [x] Backup system includes all v1.1 settings
- [x] Restore functionality for all v1.1 settings
- [x] Restart prompt appears when HAGS newly enabled

---

**Release Date:** 2026-01-10  
**Version:** 1.1  
**Build:** Enhanced Gaming Experience
