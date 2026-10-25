# Linux Fundamentals Part 2

## Overview

Part 2 extends command-line skills with SSH, command options, file operations, permissions, and common Linux directories.

## SSH and host context

SSH provides encrypted remote terminal access when the service and authentication are configured.

```bash
ssh username@host
```

Use only the host, username, and credentials supplied by the authorised lab. After connecting, confirm the remote context:

```bash
hostname
whoami
pwd
```

The AttackBox and remote lab host are separate systems. A file visible on one may not exist on the other.

## Commands, flags, and arguments

```bash
ls -la /var/log
man ls
ls --help
```

Options modify command behaviour; arguments provide inputs such as paths or filenames. Read help output when unsure.

## File operations

```bash
touch notes.txt
file notes.txt
cp notes.txt notes-copy.txt
mv notes-copy.txt archive.txt
mkdir lab-notes
```

`touch` creates an empty file if absent; `file` identifies file type; `cp` copies; `mv` moves or renames; `mkdir` creates a directory. Check destinations before moving or overwriting data.

## Permissions

Linux permissions apply to owner, group, and others, with read (`r`), write (`w`), and execute (`x`) bits.

```bash
ls -l file.txt
chmod 640 file.txt
chown user:group file.txt
```

The permission command examples are illustrative. Do not change permissions or ownership of lab evidence unless required and authorised.

## Common directories

| Path | Typical purpose |
|---|---|
| `/` | Filesystem root |
| `/home` | Users' home directories |
| `/root` | Root user's home directory |
| `/etc` | Configuration files |
| `/var/log` | Logs |
| `/tmp` | Temporary files |
| `/usr/bin` | Common executable programs on many distributions |

Exact filesystem layout varies.

## Security relevance

SSH and filesystem permissions are fundamental to system administration and investigation. Always establish the remote host and user context before interpreting files or logs.

## Key takeaways

- SSH connects to a remote host.
- Command flags and arguments affect execution.
- File operations can alter evidence.
- Least privilege limits unnecessary access.

## Official room

[Linux Fundamentals Part 2](https://tryhackme.com/room/linuxfundamentalspart2)
