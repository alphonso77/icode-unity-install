# Install Software Script

*_Note_* Choco Installs need to be run from Admin Powershell.

# Step 1 - Install Choco

`Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))`

# Step 2 - Install Software

`choco install unity-hub unity --version=2020.3.31 visualstudio2022community --package-parameters "--allWorkloads --includeRecommended --includeOptional --passive --locale en-US" -y`

## Optional - install without unity

`choco install unity-hub visualstudio2022community --package-parameters "--allWorkloads --includeRecommended --includeOptional --passive --locale en-US" -y`
