# OpenTV 1.0 (Piers)

OpenTV is an open-source TV operating system designed to run on web technologies, providing a flexible, customizable, and powerful platform for developers and users alike.

## Features
- **Sreact Programming Language**: Inspired by Swift and VB.Net, this language allows developers to write apps for OpenTV that are compiled into HTML/JS.
- **Main UI**: A Leanback-inspired interface with rounded corners and customizable backgrounds.
- **VideoRenderServer (VRS)**: System-level media playback, integrated with YouTube as the default video renderer.
- **File Manager**: Supports virtual drives (ISO/USB) and a robust error system for media playback issues.
- **App Manager**: Install and manage apps from the OpenTV repository, with apps packaged in AppPkg format.
- **Remote Control**: Wi-Fi and Bluetooth-enabled remote control features.
- **Notifications**: System-wide notifications with RTL and LTR support.
- **Recovery System**: Multiple recovery options via ISO, Wi-Fi, or Bluetooth.

## Hello World Example

Here's how to create a simple **Hello World** app using Sreact:

```swift
import GUI
import Foundation

// This is a simple Hello World app for OpenTV
func("Start") {
    GraphicalVerticalStack {
        text("Hello World!")   // Displays "Hello World!" on the screen
        button(Name="Quit"; Action=FoundationRef {
            quit(0)    // Quits the app
        })
    }
}
```

## AppPkg Format

Apps are distributed in `.AppPkg` files, which are essentially zip files containing:
- `index.html`: The main HTML file.
- `styles.css`: Optional CSS for app styling.
- `app.js`: JavaScript logic for the app.
- `metadata.xml`: XML describing the app (version, author, description).

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/Team-OpenTV/OpenTV-Core.git
   ```

2. Run OpenTV on a local server or integrate with your web environment.

3. Use the App Manager to install apps from the repository.

## Contributing

We welcome contributions! Submit your pull requests to the main repo or reach out via GitHub issues for support.

---

**Contact Us**: [GitHub Issues](https://github.com/Team-OpenTV/OpenTV-Core/issues)

---
