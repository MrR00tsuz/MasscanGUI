# Masscan GUI

A Windows Forms application that provides a graphical user interface for the Masscan port scanner. This tool makes it easy to scan IP blocks by country and analyze results with banner information.

## Features

- **Country-based IP Block Selection**: Choose a country from the dropdown to automatically fetch its IP blocks
- **Customizable Scan Settings**:
  - Port specification
  - Scan rate control
  - IP exclusion
- **Banner and Service Detection**:
  - Enable banner grabbing
  - Service scanning support
  - Filter results by banner content
- **Multiple Output Formats**:
  - IP:Port format
  - Detailed port information with banners
  - Banner-filtered results

## Requirements

- Windows operating system
- [WinPcap](https://www.winpcap.org/install/) (Required for Masscan)
- [Masscan](https://github.com/robertdavidgraham/masscan) executable (masscan64.exe)

## Installation

1. Download the latest release
2. Place `masscan64.exe` in the same directory as the GUI application
3. Install WinPcap if not already installed (use the "Download WinPcap" button in the application)
4. Run the application

## Usage

1. **Select Country**:
   - Choose a country from the dropdown to load its IP blocks
   - IP blocks will be displayed in the main text area

2. **Configure Scan**:
   - Set target ports (default: 80,3702)
   - Adjust scan rate (default: 10000)
   - Set IP addresses to exclude
   - Enable banner grabbing if needed
   - Enable service scanning if needed

3. **Run Scan**:
   - Click "Scan" to start
   - Progress will be shown in a command window
   - Use "Resume scan" if a scan was paused

4. **View Results**:
   - "IP:Port" - View results in IP:Port format
   - "IPs (port -> text file)" - Save detailed results with service information
   - "Banner Services" - Filter results by banner content

## Note

This is a GUI wrapper for Masscan. Please ensure you have proper authorization before scanning any networks or systems. Unauthorized scanning may be illegal in some jurisdictions.

## Author

[MrR00tsuz](https://github.com/MrR00tsuz)
