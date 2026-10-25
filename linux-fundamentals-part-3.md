# Linux Fundamentals Part 3

## Overview

Part 3 covers common utilities, text editors, processes, scheduled tasks, package management, and logs.

## 1. Text editors and utilities

`nano` is a terminal-based text editor. In an investigation, prefer read-only inspection unless editing is required.

```bash
date
which python3
whereis ssh
curl -I https://example.com
wget https://example.com/file.txt
```

These examples demonstrate common utilities. Use network tools only against authorised targets and verify the actual output.

## 2. Processes

A process is a running instance of a program.

```bash
ps aux
top
pgrep ssh
```

A PID identifies a process at a point in time. Investigate user, executable path, parent process, arguments, network connections, and context before deciding whether a process is suspicious. Terminating processes can disrupt services.

## 3. Cron and scheduled tasks

Cron runs commands on a schedule.

```bash
crontab -l
```

A typical cron entry contains minute, hour, day of month, month, day of week, and the command to run. System-wide schedules may be configured elsewhere depending on the distribution.

During review, record the schedule, owner, command, referenced script, and permissions. Do not execute unknown scripts simply to inspect them.

## 4. Package management

Package managers install and update software and dependencies. Debian/Ubuntu commonly use `apt`; some Fedora/RHEL-family systems use `dnf`.

```bash
apt list --installed
apt show package-name
```

These examples are distribution-specific. Package changes should follow lab instructions and authorised change procedures.

## 5. Logs and Apache access logs

Logs record system, application, and service events. Common locations include `/var/log/`, `/var/log/apache2/` on many Debian/Ubuntu Apache installations, and `/var/log/httpd/` on many RHEL-family installations. Systemd-based systems may also expose logs through `journalctl`.

```bash
ls -lah /var/log
less /var/log/apache2/access.log
tail -n 20 /var/log/apache2/access.log
grep -i 'error' /var/log/apache2/error.log
journalctl -n 50
```

Paths depend on the host, distribution, installed services, and configuration.

An Apache access log may record a client address, timestamp, request line, HTTP status, response size, and additional fields depending on the configured format. A rotated file such as `access.log.1` may represent an earlier period.

### Practical troubleshooting

If a file appears in a directory listing but cannot be read:
1. Confirm the machine with `hostname`.
2. Confirm the directory with `pwd`.
3. Check the exact name using `ls -lb`.
4. Inspect metadata with `stat filename`.
5. Read the exact error message.
6. Distinguish a missing path from permissions issues or an empty file.

Do not move logs merely to make a path match. Preserve their original context.

## Security relevance

Process inspection, scheduled-task review, package awareness, and log analysis help analysts understand what ran on a system and what activity services recorded.

## Key takeaways

- Understand process context before drawing conclusions.
- Review scheduled jobs carefully.
- Know which package manager fits the operating system.
- Treat logs as evidence and interpret them in context.
- Confirm the host before accessing files in a multi-machine lab.

## Official room

[Linux Fundamentals Part 3](https://tryhackme.com/room/linuxfundamentalspart3)
