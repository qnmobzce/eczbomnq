# MouClassInputInjection Driver Build

Standalone repository for building `MouClassInputInjection.sys` via GitHub Actions.

## Quick Start

### 1. Push to GitHub

```bash
# In your main synth repo:
git push origin master  # Push the submodule reference

# Then push the driver-build submodule:
cd submodules/driver-build
git remote add origin https://github.com/YOUR_USERNAME/synth-driver-build.git
git push -u origin master
```

### 2. Run GitHub Actions

1. Go to your repo's **Actions** tab
2. Click "Build Driver" workflow
3. Click "Run workflow"

### 3. Get the binary

**Option A: From release branch** (automatic after workflow runs)
```bash
# In main synth repo:
./fetch_driver.sh
```

**Option B: Download artifact**
- Go to the workflow run in Actions tab
- Download `MouClassInputInjection.sys` artifact
- Place in `build/` directory

## Local Build (Windows with WDK)

```batch
REM Open in Visual Studio with WDK installed
MouClassInputInjection.vcxproj

REM Build: Release | x64
REM Output: bin\x64\Release\MouClassInputInjection\MouClassInputInjection.sys
```
