# Getting Started with cs60-upmsc

Welcome to the cs60-upmsc repository! This guide will help you set up your local development environment quickly.

## 1. Clone the Repository

### Using HTTPS (Recommended for beginners):
```bash
git clone https://github.com/r4ajeti/cs60-upmsc.git
cd cs60-upmsc
```

### Using GitHub CLI:
```bash
gh repo clone r4ajeti/cs60-upmsc
cd cs60-upmsc
```


## 2. Environment Setup

* Automated activation script that handles:
* Python virtual environment creation/activation
* Dependency installation
* Environment variable loading
* Cross-platform compatibility (macOS, Linux, Windows)


### Run the Activation Script:
```bash
# Make the script executable (Unix/macOS)
chmod +x activate
# Run the activation script
. ./activate
```

#### What does the script do:

* Creates a Python virtual environment named env if it doesn't exist
* Activates the virtual environment
* Installs dependencies from requirements.txt
* Loads environment variables from .env file
* Sets up the Python path for the project

## 3. First Time Setup Checklist
Clone the repository
Run ./activate script
Verify virtual environment is active (terminal should show (cs60_env))
Check that dependencies are installed
Copy .env.example to .env and configure variables if needed

## 4. Troubleshooting
### Common Issues:
"Permission denied" when running activate:

```bash
chmod +x activate
```
#### Script not found on Windows:
Use Git Bash, WSL, or PowerShell
Ensure you're in the correct directory

#### Python not found:
Ensure Python 3.8+ is installed
Check your PATH environment variable
Virtual environment issues:

```bash
# Remove and recreate environment
rm -rf env
. ./activate
```

## 5. Daily Workflow
### Starting work session:
```bash
cd cs60-upmsc
. ./activate
```
### Ending work session:
```bash
deactivate
```
