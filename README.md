# TestNova

Automated QA tool: code analysis, live browser testing, security, 1000-user load test, accessibility, cross-browser and mobile testing - with an easy Notepad report and an AI fix prompt.

## Install on any Windows computer (one line)

**In PowerShell** paste:

```powershell
irm https://github.com/shail123-ui/TestNova/releases/latest/download/install-testnova.ps1 | iex
```

**In Command Prompt (cmd)** paste:

```bat
powershell -ExecutionPolicy Bypass -c "irm https://github.com/shail123-ui/TestNova/releases/latest/download/install-testnova.ps1 | iex"
```

After installing, open a **new** terminal. If PowerShell says "running scripts is disabled", use `testnova.cmd` instead of `testnova`.

## Install on Mac (Apple Silicon M1/M2/M3 and Intel) or Linux (one line)

Open **Terminal** and paste:

```bash
curl -fsSL https://github.com/shail123-ui/TestNova/releases/latest/download/install-testnova.sh | bash
```

No admin password needed - everything is installed into `~/.testnova`. Node.js is downloaded automatically if missing.
Then close Terminal, open a **new** one and run `testnova https://yoursite.com`. The report opens in TextEdit.
Uninstall: `rm -rf ~/.testnova`

This installs Node.js (if missing), TestNova and the test browsers (about 500 MB, one time).
Or download the 3 files from [Releases](https://github.com/shail123-ui/TestNova/releases/latest) and double-click `install-testnova.bat`.

## Use

Open a **new** terminal:

```powershell
testnova https://yoursite.com --yes          # live website (only with the owner's permission)
testnova D:\path\to\project                  # project folder: reads code + starts it + tests it
testnova http://localhost:3000 --code .      # running localhost app + its code
testnova app-release.apk                     # Android app
testnova --help                              # all options
```

The report opens automatically in Notepad.
