# Changelog – ZenOptimize

## [1.1] – Enhanced Gaming Experience
### Added
- **Windows Game Mode** – Automatically enables Game Mode for optimal gaming resource allocation
- **Hardware-Accelerated GPU Scheduling (HAGS)** – Enables GPU hardware scheduling on supported systems (Windows 10 Build 19041+)
  - Automatic Windows version detection
  - Smart detection: only prompts restart when newly enabled
  - Graceful handling for unsupported GPUs
- **Focus Assist & Notification Suppression** – Disables notifications and Focus Assist to prevent interruptions during gaming
- **Xbox Services Optimization** – Disables non-essential Xbox services (XblAuthManager, XblGameSave) while preserving controller support
- **Comprehensive logging system** – Detailed log file (ZenOptimize.log) for troubleshooting and verification
  - Timestamps for all operations
  - INFO/WARN/ERROR level logging
  - Tracks all registry modifications
- **Restart prompt dialog** – Interactive restart prompt when HAGS is enabled (required for changes to take effect)

### Changed
- Improved administrator elevation with ps2exe compatibility
- Enhanced HAGS implementation with verification and error handling
- Updated backup system to include all v1.1 settings

## [1.0] – Minimum Viable Product (MVP)
### Added
- Administrator auto-elevation (RunAs relaunch)
- Complete registry backup engine (structured backup of all edited values)
- Full rollback system (Restore-Defaults with type-aware value restoration)
- Gaming performance tweaks:
  - SystemProfile responsiveness & throttling optimization
  - SystemProfile\Tasks\Games GPU/CPU priority configuration
- GameDVR & GameBar disabling (low latency and reduced overhead)
- Network latency optimization:
  - Automatic detection of active network adapter
  - TCPNoDelay, TcpAckFrequency tuning
- Visual & background performance settings:
  - Visual effects performance mode
  - Background UWP app restriction
- Explorer/Search optimization (DisableSearchBoxSuggestions)
- Safe registry editing framework and interactive menu system
