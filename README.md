# MouClassInputInjection Driver Build

This repository contains the pre-built `MouClassInputInjection.sys` driver binary.

## Usage

### Option 1: Download pre-built binary

1. Go to the **releases** branch: `https://github.com/YOUR_USERNAME/driver-build/tree/release`
2. Download `bin/MouClassInputInjection.sys`
3. Place it in your `build/` directory alongside `load_mouii.exe`

### Option 2: Build yourself

1. Open `MouClassInputInjection.vcxproj` in Visual Studio with WDK installed
2. Build with Release|x64 configuration
3. Output: `bin/x64/Release/MouClassInputInjection/MouClassInputInjection.sys`

### Option 3: GitHub Actions

1. Go to **Actions** tab
2. Run the "Build Driver" workflow
3. Download the artifact `MouClassInputInjection.sys`

## License

Original driver by changeofpace: https://github.com/changeofpace/MouClassInputInjection
