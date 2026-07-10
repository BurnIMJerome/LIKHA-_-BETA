---
layout: default
---

# Installation Guide

## Development Or Local Desktop Install

1. Install Python dependencies:

```bat
install.bat
```

2. Start the desktop app:

```bat
run_desktop.bat
```

3. Build and run workflows from the desktop shell.

## Browser Dashboard

Start the FastAPI dashboard:

```bat
run.bat
```

Then open:

```text
http://127.0.0.1:8765
```

## Direct Server Startup

```bat
python -m uvicorn app.main:app --host 127.0.0.1 --port 8765
```

## Desktop Build

```bat
build_desktop.bat
```

Packaged output:

```text
dist\Likha\Likha.exe
```

## Installer Build

```bat
build_installer.bat
```

Installer output:

```text
installer-output\LikhaSetup.exe
```

## OCR Setup

OCR activities prefer the bundled Tesseract folder:

```text
tesseract/
  tesseract.exe
  tessdata/
    eng.traineddata
```

See:

[How to Setup OCR Tesseract](How%20to%20Setup%20OCR%20Tesseract.html)

## Robot Runtime

For unattended setup:

- `run_robot_service.bat`
- `install_robot_service.bat`
- `run_user_agent.bat`

See:

- [Robot Service and User Agent.md](Robot%20Service%20and%20User%20Agent.html)
- [Distributed Control Room and VM Robot Setup.md](Distributed%20Control%20Room%20and%20VM%20Robot%20Setup.html)


