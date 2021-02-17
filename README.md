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

 * [2021-02-16] - Corrected credits in the beginning of the script. I originally copied another script and simply started modifying the functions.
