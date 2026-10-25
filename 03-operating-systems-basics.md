# Pre Security — Operating Systems Basics

## Module overview

This module introduces operating systems, Windows and Linux basics, command-line interfaces, and operating-system security.

## 1. What an operating system does

An OS manages processes, memory, filesystems, user accounts, devices, networking, and application access to hardware. It also provides mechanisms for authentication, permissions, logging, and system administration.

## 2. Windows basics

Windows provides a graphical interface and command-line tools for interacting with files, processes, services, users, and settings. Understanding Windows is important because it is widely deployed on enterprise endpoints and servers.

## 3. Linux CLI basics

The shell interprets commands entered in a terminal. Useful orientation commands include:

```bash
whoami
hostname
pwd
ls -la
cd /var/log
```

- `whoami`: current account
- `hostname`: machine name
- `pwd`: current directory
- `ls -la`: list files including hidden entries
- `cd`: change directory

Always establish which machine you are using. A browser-based AttackBox and a remote lab host have separate filesystems.

## 4. Windows CLI basics

Windows provides tools such as Command Prompt and PowerShell. They can inspect files, processes, network configuration, and system state. PowerShell is also an automation environment with structured objects and cmdlets.

Examples:

```powershell
whoami
hostname
Get-Location
Get-ChildItem
Get-Process
```

The exact commands available depend on the shell and permissions.

## 5. Operating-system security

Important practices include least privilege, strong authentication, patching, secure configuration, service minimisation, logging, and controlled access to files and processes.

## Filesystem troubleshooting

If a path fails:
1. Confirm the host (`hostname`).
2. Confirm the working directory (`pwd` or `Get-Location`).
3. Verify the exact name and path.
4. Check permissions and object type.
5. Read the exact error before drawing conclusions.

A hidden filename is not an access-control mechanism. An empty file, missing file, and permission error are different conditions.

## Security relevance

Host investigation often begins by identifying the host, user, current directory, processes, services, and relevant logs.

## Key takeaways

- Operating systems coordinate hardware and applications.
- Linux and Windows both provide CLI tools for administration and investigation.
- Host context matters when investigating files or logs.
- Permissions and secure configuration are fundamental controls.

## Rooms covered by this module

- Operating Systems: Introduction
- Windows Basics
- Linux CLI Basics
- Windows CLI Basics
- Operating System Security

## Official reference

[TryHackMe Pre Security](https://tryhackme.com/path/outline/presecurity)
