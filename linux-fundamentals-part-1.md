# Linux Fundamentals Part 1

## Overview

Part 1 introduces Linux and the terminal, including orientation commands, directory navigation, file reading, hidden files, file search, and shell operators.

## Orientation and navigation

```bash
whoami
hostname
pwd
ls -la
cd /var/log
cd ..
```

- `whoami` shows the current account.
- `hostname` shows the machine name.
- `pwd` prints the current working directory.
- `ls -la` lists files, including dot-prefixed entries.
- `cd` changes directories; `..` means the parent directory.

A path beginning with `/` is absolute. A relative path is interpreted from the current directory.

## Reading and searching files

```bash
cat file.txt
less file.txt
head -n 10 file.txt
tail -n 20 file.txt
grep -i 'error' application.log
find /var/log -type f -name 'access.log' 2>/dev/null
```

Use `less` for long files and `tail` for recent log entries. `grep` searches file content; `find` searches for paths. Suppressing error output can hide permission problems, so use `2>/dev/null` intentionally.

## Hidden files

In Unix-like systems, filenames beginning with `.` are typically hidden from ordinary directory listings. Use `ls -a` to show them. The naming convention does not protect the file from unauthorised access.

## Shell operators

- `>` redirects output and overwrites the destination.
- `>>` appends output.
- `|` passes output to another command.
- `&&` runs the next command only if the previous one succeeds.
- `;` separates sequential commands.

Redirection can overwrite data, so inspect commands before running them.

## Security relevance

These commands support initial host triage: establish the machine and user, locate relevant files, read logs, and search for indicators. Avoid changing evidence unless the task requires it.

## Key takeaways

- Confirm context before investigating.
- Use absolute and relative paths correctly.
- Choose a suitable command for the file size and task.
- Distinguish hidden, missing, empty, and inaccessible files.

## Official room

[Linux Fundamentals Part 1](https://tryhackme.com/room/linuxfundamentalspart1)
