# ThinClient Setup for Pi

This is a tutorial about how to configure a Pi for use as a ThinClient.

## Installation

```bash
git clone https://github.com/LouisOuellet/ThinClient-for-Pi
cd ThinClient-for-Pi
# Default not secured
./setup
# To lock down add a user
./setup -u admin
```

## Help

```bash
./setup -?
Invalid option: ?

Usage: setup [options]

Options:

-h                     => Set Hostname
-u                     => Set Username
-p                     => Set Password
-o                     => Set openVPN
-v                     => Enable Verbose Mode
                          Input commands sent are stored in log/setup/
```

## Changelog

 * [2021-02-18] - Added the package dnsutils to the installation process
 * [2021-02-18] - Added the uninstallation of rdp if already install
 * [2021-02-18] - Added verifications on /boot/config.txt before modifying it
 * [2021-02-18] - Corrected a typo when running all mkdir command. was using P instead of p.
 * [2021-02-18] - Added --disabled-password --gecos '' to the creation of user to run adduser non-interactively
 * [2021-02-18] - If debug Verbose mode is active, the script will now tell you where the log is saved
 * [2021-02-18] - Now empties the /etc/skel directory before starting the its setup
 * [2021-02-18] - Added sudo to mkdir commands
 * [2021-02-18] - Corrected an error with the log directory variable. Causing it to constantly change and thus stopping the script due to missing file error.
 * [2021-02-18] - Corrected an error in the openVPN setup. I was trying a else if, but bash did not seem to tolerate it. The openVPN setup should not be attempted yet. Since it is not complete.
 * [2021-02-16] - Corrected credits in the beginning of the script. I originally copied another script and simply started modifying the functions.
