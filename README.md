# AIO-IT-TOOLS-v0.13.2

AIO IT TOOLS is a Windows maintenance and diagnostics utility built with Python and PySide6.

This release fixes the latest source-launch blocker, cleans up release metadata, and keeps the project wording polished and professional.

Fixed
Fixed launch error:
ModuleNotFoundError: No module named 'core.release'
Added core/release.py as the stable release metadata module.
Kept core/beta.py as a compatibility wrapper for older imports.
Updated UI imports to use core.release.
Removed portfolio-specific wording from visible project files.
Updated README with clean project/GitHub wording.
Version bumped to 0.13.2.
Current Features
Home dashboard
App update scan
Optional winget provider
Windows Update health checks
Conservative Windows Update service repair
Driver update comparison
Driver review and guarded automation
Cleaner with safe defaults
Advanced cleanup toggle
Repair tools with advanced toggle
Wi-Fi profiles and local password display
Health scan page
Reports
Runtime self-test
Support ZIP export
System Notes page
Privacy and Safety
Wi-Fi passwords are not stored.
Sensitive values are redacted from Support ZIP/log output where possible.
Driver automation requires review and high-confidence matches.
Source code remains readable and reviewable.
Running from Source
run_aio_it_tools.bat
Building the EXE
build_exe.bat

Expected output:

dist\AIOITTools.exe
Release File

Attach:

aio_it_tools_v0132.zip
