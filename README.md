![Banner](banner.png)

# misconfig-ConfigSecretScanner
Scans configuration files for embedded secrets (API keys, passwords, etc.) using regex patterns and entropy analysis. - Focused on Check for misconfigurations in configuration files or infrastructure definitions

Findings store only a 20 character snippet of a match, in the console, the log, and the `-j` JSON output, never the full matched text. A run that cannot read a file it was asked to scan, or a file inside a directory it was asked to scan, exits 1 and names the unreadable file, instead of reporting that no secrets were found.

## Install
`git clone https://github.com/ShadowGuardAI/misconfig-configsecretscanner`

## Usage
`./misconfig-configsecretscanner [params]`

## Parameters
- `-h`: Show help message and exit
- `-r`: Recursively scan directories.
- `-e`: List of directories or files to exclude from the scan.
- `-v`: Enable verbose output.
- `-j`: Path to save JSON output.

## License
Copyright (c) ShadowGuardAI
