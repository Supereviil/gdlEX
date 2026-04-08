# gdlEX — GUI Frontend for gallery-dl (Alpha Test Release)

## Overview
**gdlEXi** is a Windows desktop application that provides a graphical interface for `gallery-dl`, allowing users to download images, videos, and other media without using command-line arguments. This tool is intended for testing and feedback during early development.

---

## What the Program Does
* **Full GUI Wrapper:** A complete interface around `gallery-dl.exe`.
* **Flexible Downloading:** Supports both single URL downloads and multi-URL batch queues.
* **Argument Builder:** Automatically constructs `gallery-dl` arguments based on your UI settings.
* **Live Monitoring:** Displays real-time console output and file counts.
* **Session Management:** Saves and restores your URL queue and output folder between launches.
* **Process Control:** Allows pausing and resuming of active downloads.
* **Safe Termination:** Uses Windows Job Objects for clean process stopping.
* **Portable Settings:** Saves all configurations to a local `.ini` file.

---

## Features Added Beyond gallery-dl
These features are unique to this GUI and operate as post-processing or pre-processing steps:

### Rename and Sanitization Tools
* **Emoji Removal:** Strip emojis from filenames.
* **Punctuation Removal:** Clean up filenames by removing special characters.
* **Space Management:** Remove or replace spaces in filenames.
* **Custom String Removal:** Target and delete specific text patterns.
* **Length Trimming:** Enforce a maximum character length for filenames to avoid OS errors.
* **Extension Swapping:** Change file extensions automatically (e.g., `.m4v` to `.mp4`).

### CBZ Archiving
* Automatically compress downloaded folders into `.cbz` (Comic Book Zip) archives upon completion.

### Cookie Extraction UI
* Extract cookies directly from installed browsers.
* Optionally select a local cookie file manually.

### Filename Template Builder
Presets including:
* Default
* Original filename
* ID only
* Date + filename
* Username + ID
* Category + ID
* Custom template support

### Multi-URL Queue Mode
* Paste a list of URLs for sequential processing.
* Automatic subfolder creation for each gallery.
* Progress tracking ensures the queue resumes where you left off if interrupted.

### Output Logging
* Optionally save a `.log` file to the output directory after each successful download.

---

## Requirements
* **OS:** Windows 10 or Windows 11.
* **Core Dependency:** `gallery-dl.exe` must be placed in the same folder as this program.
* **Python:** A Python installation may be required depending on your specific `gallery-dl` setup.

## Installation
1.  Download the ZIP release.
2.  Extract the contents to a folder of your choice.
3.  **Important:** Place your `gallery-dl.exe` binary in the same folder as `g-dlphi.exe`.
4.  Run `g-dlphi.exe`.

---

## Known Limitations (Alpha)
* Only Windows is supported at this time (macOS and Linux versions are planned).
* Certain rename operations may behave differently depending on specific site filename structures.
* Output parsing is currently basic and may not detect 100% of file events.
* UI polish and error handling are ongoing and will improve in future builds.

## Feedback & Bug Reports
If you find a bug or want to request a feature, please open an issue and I will review it.

---

## Disclaimer
* This program is a third-party GUI and is **not** affiliated with, endorsed by, or sponsored by `gallery-dl` or its developers.
* `gallery-dl` is the property of its respective owner(s).
* This program does not modify, redistribute, or include the `gallery-dl` binary.
* Users are responsible for complying with the Terms of Service of any website they download from.
* The author is not responsible for any misuse of `gallery-dl` or this application.
