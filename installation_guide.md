# Development Tools Installation Guide for Windows 11

## 1. Install Git

1. Download Git:
   - Visit [Git for Windows](https://git-scm.com/download/win)
   - Click on "Click here to download" for the latest version
   - The download will start automatically

2. Install Git:
   - Run the downloaded `.exe` file
   - Accept the license agreement
   - Keep default installation settings (recommended for beginners)
   - Choose default editor (Notepad recommended for beginners)
   - Select "Git from the command line and also from 3rd-party software"
   - Choose "Use the OpenSSL library" for HTTPS
   - Select "Checkout Windows-style, commit Unix-style line endings"
   - Choose "Use Windows' default console window"
   - Keep other default options
   - Click "Install"

3. Verify Installation:
   - Open PowerShell
   - Type `git --version`
   - You should see the Git version number

## 2. Install GitHub Desktop

1. Download GitHub Desktop:
   - Visit [GitHub Desktop](https://desktop.github.com/)
   - Click "Download for Windows"

2. Install GitHub Desktop:
   - Run the downloaded `.exe` file
   - The installation will proceed automatically
   - Sign in with your GitHub account when prompted
   - Configure your Git settings with your name and email

## 3. Install Visual Studio Code

1. Download VS Code:
   - Visit [Visual Studio Code](https://code.visualstudio.com/)
   - Click "Download for Windows"

2. Install VS Code:
   - Run the downloaded installer
   - Accept the agreement
   - Important: Check these options during installation:
     - [x] Add "Open with Code" action to Windows Explorer file context menu
     - [x] Add "Open with Code" action to Windows Explorer directory context menu
     - [x] Register Code as an editor for supported file types
     - [x] Add to PATH

3. Recommended Extensions:
   - Python
   - Git Graph
   - GitLens
   - Material Icon Theme

## 4. Install Python

1. Download Python:
   - Visit [Python Downloads](https://www.python.org/downloads/)
   - Click "Download Python" (latest stable version)
   - The download will start automatically

2. Install Python:
   - Run the downloaded installer
   - Important: Check "Add Python to PATH"
   - Click "Install Now" (recommended)
   - Wait for the installation to complete

3. Verify Installation:
   - Open PowerShell
   - Type `python --version`
   - Also verify pip: `pip --version`

## Post-Installation Setup

1. Configure Git:
```powershell
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

2. Basic Python Setup:
```powershell
# Create and activate virtual environments
python -m pip install --upgrade pip
pip install virtualenv
```

3. VS Code Python Setup:
   - Open VS Code
   - Install Python extension
   - Press `Ctrl+Shift+P`
   - Type "Python: Select Interpreter"
   - Choose your installed Python version

## Verification Steps

1. Git Setup:
```powershell
git --version
```

2. Python Setup:
```powershell
python --version
pip --version
```

3. VS Code Setup:
   - Open VS Code
   - Open Terminal (`Ctrl+~`)
   - Verify Git integration by running `git --version`
   - Verify Python integration by running `python --version`

## Troubleshooting

- If commands aren't recognized, restart your terminal or computer
- Ensure all "Add to PATH" options were selected during installation
- For Git/GitHub issues, verify your credentials in GitHub Desktop
- For Python path issues, manually add Python to system environment variables
