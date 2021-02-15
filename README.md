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
-v                     => Enable dbg Mode
                          Input commands sent are stored in log/setup/
```
