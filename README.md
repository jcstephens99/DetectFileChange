# Detect File Change

A script to check if a certain file has been changed.

## Requirements
* `bash`
* `readlink` (comes with GNU's `coreutils`)

## Installation
Simpily copy the `detect_file_change` script from this repository's `usr/bin` directory to anywhere you wish to execute it from.

## Usage
`detect_file_change [file_to_check]`

## Directories/Files
By default, this program will use the `/var/lib/dfc` directory to keep track of file state and will log any changes found to `/var/log/dfc.log`. This is changeable by via the variables at the top the of script.

These paths will be automatically made at runtime if they do not exist already.

## Cron
This repository also includes a quick example cron.d file, which will check /etc/passwd every fifteen minutes
