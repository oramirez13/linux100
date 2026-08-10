# Linux commands guide - Arch Linux edition

## 1. System information

| Command       | Explanation                                                              |
| ------------- | ------------------------------------------------------------------------ |
| `uname -a`    | Shows complete kernel and system information.                            |
| `hostname`    | Shows the computer name.                                                 |
| `hostnamectl` | Shows detailed system information and allows changing the hostname.      |
| `arch`        | Shows the system architecture.                                           |
| `lscpu`       | Shows processor information.                                             |
| `free -h`     | Shows RAM and swap usage.                                                |
| `uptime`      | Shows how long the system has been running.                              |
| `date`        | Shows the current date and time.                                         |
| `whoami`      | Shows the current user.                                                  |
| `id`          | Shows the UID, GID, and groups of the user.                              |

---

# 2. Navigating the file system

| Command  | Explanation                                             |
| -------- | ------------------------------------------------------- |
| `pwd`    | Shows the current directory.                            |
| `ls`     | Lists the contents of the directory.                    |
| `ls -la` | Lists all files with details.                           |
| `cd`     | Changes the directory.                                  |
| `tree`   | Shows the directory structure as a tree.                |
| `mkdir`  | Creates a directory.                                    |
| `rmdir`  | Removes an empty directory.                             |
| `touch`  | Creates an empty file.                                  |
| `cp`     | Copies files or directories.                            |
| `mv`     | Moves or renames files.                                 |
| `rm`     | Removes files or directories.                           |
| `find`   | Finds files and directories.                            |
| `locate` | Finds files using an indexed database.                  |

---

# 3. Viewing files

| Command   | Explanation                                  |
| --------- | -------------------------------------------- |
| `cat`     | Shows the complete content of a file.        |
| `less`    | Views files page by page.                    |
| `head`    | Shows the first lines of a file.             |
| `tail`    | Shows the last lines of a file.              |
| `tail -f` | Follows a file in real time.                 |
| `file`    | Identifies the type of a file.               |
| `stat`    | Shows detailed information about a file.     |

---

# 4. Searching and processing text

| Command   | Explanation                             |
| --------- | --------------------------------------- |
| `grep`    | Searches text using patterns.           |
| `grep -r` | Searches text recursively.              |
| `awk`     | Processes text by columns.              |
| `sed`     | Edits and transforms text.              |
| `cut`     | Extracts columns of text.               |
| `sort`    | Sorts lines.                            |
| `uniq`    | Removes consecutive duplicate lines.    |
| `tr`      | Replaces characters.                    |
| `wc`      | Counts lines, words, and characters.    |

---

# 5. Permissions

| Command | Explanation                                    |
| ------- | ---------------------------------------------- |
| `chmod` | Changes permissions of files and directories.  |
| `chown` | Changes the owner.                             |
| `chgrp` | Changes the owner group.                       |
| `umask` | Defines the default permissions.               |

---

# 6. Users

| Command  | Explanation                                       |
| -------- | ------------------------------------------------- |
| `who`    | Shows connected users.                            |
| `w`      | Shows users and active processes.                 |
| `groups` | Shows the groups of the user.                     |
| `passwd` | Changes a user password.                          |
| `sudo`   | Runs commands with administrative privileges.     |
| `visudo` | Safely edits the sudoers file.                    |

---

# 7. Processes

| Command   | Explanation                          |
| --------- | ------------------------------------ |
| `ps`      | Shows running processes.             |
| `ps aux`  | Lists all processes.                 |
| `top`     | Real-time process monitor.           |
| `htop`    | Interactive process monitor.         |
| `kill`    | Terminates a process by its PID.     |
| `killall` | Terminates processes by name.        |
| `pgrep`   | Searches processes by name.          |
| `pkill`   | Terminates processes by name.        |

---

# 8. Services (systemd)

| Command                      | Explanation                       |
| ---------------------------- | --------------------------------- |
| `systemctl status service`   | Shows the status of a service.    |
| `systemctl start service`    | Starts a service.                 |
| `systemctl stop service`     | Stops a service.                  |
| `systemctl restart service`  | Restarts a service.               |
| `systemctl enable service`   | Enables automatic startup.        |
| `systemctl disable service`  | Disables automatic startup.       |

---

# 9. Logs

| Command          | Explanation                                |
| ---------------- | ------------------------------------------ |
| `journalctl`     | Shows system logs.                         |
| `journalctl -b`  | Shows logs of the current boot.            |
| `journalctl -xe` | Shows recent errors.                       |
| `journalctl -f`  | Follows the log in real time.              |
| `dmesg`          | Shows kernel messages.                     |

---

# 10. Networking

| Command     | Explanation                                |
| ----------- | ------------------------------------------ |
| `ip addr`   | Shows the network interfaces.              |
| `ip route`  | Shows the routing table.                   |
| `ping`      | Checks connectivity with a host.           |
| `ss -tulnp` | Shows open ports and connections.          |
| `curl`      | Makes HTTP requests.                       |
| `wget`      | Downloads files from the Internet.         |
| `dig`       | Queries DNS records.                       |
| `host`      | Resolves DNS names.                        |
| `nmcli`     | Manages NetworkManager from the terminal.  |

---

# 11. SSH

| Command            | Explanation                         |
| ------------------ | ----------------------------------- |
| `ssh user@host`    | Connects to a remote server.        |
| `scp`              | Copies files over SSH.              |
| `sftp`             | Transfers files over SSH.           |
| `ssh-keygen`       | Generates SSH keys.                 |
| `ssh-copy-id`      | Copies the public key to the server.|

---

# 12. Disks

| Command          | Explanation                                 |
| ---------------- | ------------------------------------------- |
| `lsblk`          | Lists disks and partitions.                 |
| `df -h`          | Shows the disk space available.             |
| `du -sh folder`  | Shows the size of a folder.                 |
| `blkid`          | Shows UUID and file system type.            |
| `mount`          | Mounts a file system.                       |
| `umount`         | Unmounts a file system.                     |

---

# 13. Compression

| Command  | Explanation                |
| -------- | -------------------------- |
| `tar`    | Packages files.            |
| `gzip`   | Compresses files.          |
| `gunzip` | Decompresses GZIP files.   |
| `zip`    | Compresses in ZIP format.  |
| `unzip`  | Extracts ZIP files.        |

---

# 14. Package management (Arch Linux)

## Pacman

| Command               | Explanation                                     |
| --------------------- | ----------------------------------------------- |
| `pacman -Syu`         | Fully updates the system.                       |
| `pacman -S package`   | Installs a package.                             |
| `pacman -R package`   | Removes a package.                              |
| `pacman -Rns package` | Removes a package and unnecessary dependencies. |
| `pacman -Qs name`     | Searches installed packages.                    |
| `pacman -Qi package`  | Shows information about a package.              |
| `pacman -Q`           | Lists all installed packages.                   |
| `pacman -Sc`          | Cleans the package cache.                       |

## Yay

| Command            | Explanation                                                 |
| ------------------ | ----------------------------------------------------------- |
| `yay -Syu`         | Updates official and AUR packages.                          |
| `yay -S package`   | Installs a package from the AUR or official repositories.   |
| `yay -Rns package` | Removes a package and its dependencies.                     |
| `yay -Qs name`     | Searches packages.                                          |

---

# 15. Audit and security

| Command      | Explanation                            |
| ------------ | -------------------------------------- |
| `auditctl`   | Manages audit rules.                   |
| `ausearch`   | Searches events logged by auditd.      |
| `aureport`   | Generates audit reports.               |
| `journalctl` | Reviews system events.                 |
| `sha256sum`  | Calculates the SHA-256 hash of a file. |
| `gpg`        | Signs and encrypts files.              |

---

# 16. Diagnostics

| Command   | Explanation                                    |
| --------- | ---------------------------------------------- |
| `lsof`    | Lists files opened by processes.               |
| `strace`  | Shows the system calls of a process.           |
| `tcpdump` | Captures network traffic.                      |
| `vmstat`  | Shows memory and CPU statistics.               |
| `iostat`  | Shows disk statistics.                         |

---

# 17. Help

| Command           | Explanation                                        |
| ----------------- | -------------------------------------------------- |
| `man command`     | Opens the manual of a command.                     |
| `command --help`  | Shows the quick help of a command.                 |
| `info command`    | Opens GNU documentation if available.              |
| `apropos word`    | Searches commands related to a keyword.            |
