g-dlphi — GUI Frontend for gallery-dl (Alpha Test Release)

Overview
g-dlphi is a Windows desktop application that provides a graphical interface for gallery-dl, allowing users to download images, videos, and other media without using command-line arguments. This tool is intended for testing and feedback during early development.

What the Program Does
• Provides a full GUI wrapper around gallery-dl.exe
• Supports single URL downloads
• Supports multi-URL batch downloading
• Automatically builds gallery-dl arguments based on user settings
• Displays live output and file counts
• Saves and restores sessions (URLs and output folder)
• Allows pausing and resuming downloads
• Uses Windows Job Objects for safe process termination
• Saves all settings to an INI file

Features Added Beyond gallery-dl
These features are not part of gallery-dl and are unique to this GUI:

Rename and Sanitization Tools
• Remove emojis
• Remove punctuation
• Remove spaces
• Remove a custom string
• Trim filenames to a maximum length
• Swap file extensions (example: m4v to mp4)

CBZ Archiving
• Automatically compress downloaded folders into .cbz comic archives

Cookie Extraction UI
• Extract cookies from installed browsers
• Or select a cookie file manually

Filename Template Builder
• Default
• Original filename
• ID only
• Date + filename
• Username + ID
• Category + ID
• Custom template

Multi-URL Queue Mode
• Paste a list of URLs
• Automatically creates subfolders
• Saves progress between sessions
• Resumes where you left off

Output Logging
• Optionally save a log file to the output directory after each download

Requirements
• Windows 10 or Windows 11
• gallery-dl.exe must be placed in the same folder as this program
• Python installation if required by your gallery-dl setup

Installation

    Download the ZIP release

    Extract it anywhere

    Place gallery-dl.exe in the same folder as this program

    Run g-dlphi.exe

Known Limitations (Alpha)
• Only Windows is supported at this time
• macOS and Linux versions are planned
• Some rename operations may behave differently depending on filenames
• Output parsing is basic and may not detect all file events
• Folder structuring is a bit off, will be tweaked in the future
• UI polish and error handling will improve over time

Future Plans
• Name Change (g-dlphi is only temporary)
• New Icon

Contact for Requests and Bug Reports
If you find a bug or want to request a feature, open an issue and I'll have a look


Disclaimer
This program is a third-party GUI and is not affiliated with, endorsed by, or sponsored by gallery-dl or its developers.
gallery-dl is the property of its respective owner(s).
This program does not modify, redistribute, or include gallery-dl.
Users are responsible for complying with the Terms of Service of any website they download from.
The author of this program is not responsible for misuse of gallery-dl or this application.