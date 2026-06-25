# AIO IT TOOLS v0.13.2 — Gold Master Launch Fix

**AIO IT TOOLS** is a Windows maintenance and diagnostics utility built with **Python** and **PySide6**. It provides a clean desktop interface for common IT support tasks, including update checks, repair tools, driver review, cleanup workflows, health scans, reports, and support diagnostics.

This release fixes the latest source-launch issue, cleans up release metadata, and keeps the project wording polished and professional.

## What’s Fixed in v0.13.2

Fixed the source launch error:

```text
ModuleNotFoundError: No module named 'core.release'
```

Changes included:

* Added `core/release.py` as the stable release metadata module.
* Kept `core/beta.py` as a compatibility wrapper for older imports.
* Updated UI imports to use `core.release`.
* Removed portfolio-specific wording from visible project files.
* Updated the README with cleaner GitHub/project wording.
* Bumped the application version to `0.13.2`.

## Current Features

* Home dashboard
* App update scan
* Optional `winget` provider
* Windows Update health checks
* Conservative Windows Update service repair
* Driver update comparison
* Driver review workflow
* Guarded driver automation for high-confidence matches only
* Cleaner tools with safe defaults
* Advanced cleanup toggle
* Repair tools with advanced toggle
* Wi-Fi profile viewer with local password display
* Health scan page
* Reports page
* Runtime self-test
* Support ZIP export
* System Notes page

## Privacy and Safety

AIO IT TOOLS is designed with safety and transparency in mind.

* Wi-Fi passwords are not stored.
* Sensitive values are redacted from Support ZIP/log output where possible.
* Driver automation requires user review and high-confidence matches.
* Advanced cleanup and repair tools are gated behind toggles.
* Source code remains readable and reviewable.
* Windows/system-changing actions require confirmation.

## Running from Source

```bat
run_aio_it_tools.bat
```

The launcher checks for required Python packages and starts the application from source.

## Building the EXE

```bat
build_exe.bat
```

Expected output:

```text
dist\AIOITTools.exe
```

## Unsigned Build Notice

This build is unsigned. Windows may show a SmartScreen or antivirus reputation warning for unsigned executables.

For review or testing, you can run the project from source or build the executable locally.

## System Notes

Some behavior depends on Windows components and local system policy:

* Windows Update may be restricted by organization or system policy.
* `winget` depends on Microsoft App Installer.
* Unsigned executables may trigger reputation warnings.
* Wi-Fi password display depends on Windows `netsh`, administrator permissions, and local security policy.

## Release File

Attach the latest ZIP:

```text
aio_it_tools_v0132.zip
```
