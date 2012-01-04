# Overview
This repository contains a number of nagios plugins I've written from scratch when I could not find an existing plugin that did what I needed.

## check_aacraid
### Usage
    check_aacraid
### Requirements
    The arcconf program from Areca.

## check_md
### Usage
    check_md
### Requirements
  * Linux
  * mdadm

## check_nfs_mount
### Usage
    check_nfs_mount /mountpoint
### Requirements
  * Linux
  * Perl
  * Proc::ProcessTable

## check_process_memory
### Usage
    check_process_memory -n program_name -w warning_level -c critical_level
### Requirements
  * Linux
  * Perl
  * Proc::ProcessTable
  * Getopt::Long
  * Pod::Usage
  * Readonly

## check_scsi
### Usage
    check_scsi
### Requirements
    Linux

## check_swapping
### Usage
    check_swapping  [ --delay=<delay between samples> ] \
    [ --in_warning=<page in warning threshold> ] [ --in_critical=<page in critical threshold> ]  \
    [ --out_warning=<page out warning threshold> ] [ --out_critical=<page out critical threshold> ]
### Requirements
  * Linux
  * Perl
  * Nagios::Plugin

# Licensing

The shell scripts are released into the public domain using [CC0 1.0 Universal](http://creativecommons.org/publicdomain/zero/1.0/legalcode).

The perl scripts are released under the GPL; see COPYING.
