# Ubuntu Commands Cheat Sheet

## File and Directory Operations

| Command | Description |
|---------|-------------|
| `ls` | List directory contents |
| `ls -la` | List all files including hidden, with detailed info |
| `cd [dir]` | Change directory |
| `cd ~` | Change to home directory |
| `cd ..` | Move up one directory |
| `pwd` | Print working directory path |
| `mkdir [dir]` | Create directory |
| `mkdir -p [path]` | Create directory with parent directories |
| `rmdir [dir]` | Remove empty directory |
| `rm [file]` | Remove file ⚠️ |
| `rm -r [dir]` | Remove directory and contents recursively ⚠️ |
| `rm -rf [dir]` | Force remove directory and contents ⚠️ **DANGEROUS** |
| `cp [src] [dest]` | Copy file |
| `cp -r [src] [dest]` | Copy directory recursively |
| `mv [src] [dest]` | Move/rename file or directory |
| `find [path] -name [pattern]` | Find files by name |
| `find [path] -type f` | Find files only |
| `locate [filename]` | Find files using database |
| `which [command]` | Show path of command |

## File Viewing and Editing

| Command | Description |
|---------|-------------|
| `cat [file]` | Display file contents |
| `less [file]` | View file with pagination |
| `more [file]` | View file page by page |
| `head [file]` | Show first 10 lines of file |
| `head -n [num] [file]` | Show first n lines |
| `tail [file]` | Show last 10 lines of file |
| `tail -f [file]` | Follow file changes in real-time |
| `nano [file]` | Edit file with nano editor |
| `vim [file]` | Edit file with vim editor |
| `grep [pattern] [file]` | Search for pattern in file |
| `grep -r [pattern] [dir]` | Search recursively in directory |

## File Permissions and Ownership

| Command | Description |
|---------|-------------|
| `chmod [permissions] [file]` | Change file permissions |
| `chmod +x [file]` | Make file executable |
| `chmod 755 [file]` | Set permissions (owner: rwx, group/other: rx) |
| `chown [user] [file]` | Change file owner |
| `chown [user]:[group] [file]` | Change owner and group |
| `chgrp [group] [file]` | Change file group |
| `umask` | Display default permissions |

## System Information

| Command | Description |
|---------|-------------|
| `whoami` | Display current username |
| `id` | Display user and group IDs |
| `uname -a` | System information |
| `hostnamectl` | Display system hostname info |
| `uptime` | Show system uptime and load |
| `date` | Display current date and time |
| `cal` | Display calendar |
| `df -h` | Show disk space usage (human readable) |
| `du -h [dir]` | Show directory size |
| `free -h` | Display memory usage |
| `lscpu` | Display CPU information |
| `lsblk` | List block devices |
| `lsusb` | List USB devices |
| `lspci` | List PCI devices |

## Process Management

| Command | Description |
|---------|-------------|
| `ps aux` | Show all running processes |
| `ps -ef` | Show processes in full format |
| `top` | Display running processes (interactive) |
| `htop` | Enhanced process viewer (if installed) |
| `jobs` | Show active jobs |
| `bg` | Put job in background |
| `fg` | Bring job to foreground |
| `nohup [command] &` | Run command immune to hangups |
| `kill [PID]` | Terminate process by ID |
| `kill -9 [PID]` | Force kill process ⚠️ |
| `killall [process_name]` | Kill all processes by name ⚠️ |
| `pgrep [pattern]` | Find process ID by name |
| `pkill [pattern]` | Kill processes by name pattern ⚠️ |

## Network Commands

| Command | Description |
|---------|-------------|
| `ping [host]` | Test network connectivity |
| `wget [url]` | Download file from web |
| `curl [url]` | Transfer data from server |
| `ssh [user]@[host]` | Connect to remote host via SSH |
| `scp [file] [user]@[host]:[path]` | Copy file over SSH |
| `netstat -tulpn` | Show network connections |
| `ss -tulpn` | Modern netstat alternative |
| `iptables -L` | List firewall rules |
| `ufw status` | Check UFW firewall status |

## Package Management (APT)

| Command | Description |
|---------|-------------|
| `sudo apt update` | Update package lists |
| `sudo apt upgrade` | Upgrade installed packages |
| `sudo apt install [package]` | Install package |
| `sudo apt remove [package]` | Remove package |
| `sudo apt purge [package]` | Remove package and config files |
| `sudo apt autoremove` | Remove unnecessary packages |
| `sudo apt search [term]` | Search for packages |
| `apt list --installed` | List installed packages |
| `apt show [package]` | Show package information |
| `sudo dpkg -i [package.deb]` | Install .deb package |

## Archive and Compression

| Command | Description |
|---------|-------------|
| `tar -czf [archive.tar.gz] [files]` | Create compressed archive |
| `tar -xzf [archive.tar.gz]` | Extract compressed archive |
| `tar -tf [archive.tar.gz]` | List archive contents |
| `zip -r [archive.zip] [directory]` | Create ZIP archive |
| `unzip [archive.zip]` | Extract ZIP archive |
| `gzip [file]` | Compress file |
| `gunzip [file.gz]` | Decompress file |

## Text Processing

| Command | Description |
|---------|-------------|
| `sort [file]` | Sort lines in file |
| `uniq [file]` | Remove duplicate lines |
| `wc [file]` | Count lines, words, characters |
| `cut -d'[delimiter]' -f[field] [file]` | Extract columns from file |
| `awk '{print $1}' [file]` | Print first column |
| `sed 's/old/new/g' [file]` | Replace text in file |
| `diff [file1] [file2]` | Compare files |
| `comm [file1] [file2]` | Compare sorted files |

## Input/Output and Redirection

| Command | Description |
|---------|-------------|
| `[command] > [file]` | Redirect output to file (overwrite) |
| `[command] >> [file]` | Redirect output to file (append) |
| `[command] < [file]` | Use file as input |
| `[command1] \| [command2]` | Pipe output to another command |
| `tee [file]` | Write output to both file and stdout |

## System Control and Services

| Command | Description |
|---------|-------------|
| `sudo systemctl start [service]` | Start service |
| `sudo systemctl stop [service]` | Stop service |
| `sudo systemctl restart [service]` | Restart service |
| `sudo systemctl enable [service]` | Enable service at boot |
| `sudo systemctl disable [service]` | Disable service at boot |
| `systemctl status [service]` | Check service status |
| `systemctl list-units --type=service` | List all services |
| `sudo reboot` | Restart system ⚠️ |
| `sudo shutdown -h now` | Shutdown system ⚠️ |

## Environment and Variables

| Command | Description |
|---------|-------------|
| `env` | Display environment variables |
| `export [VAR=value]` | Set environment variable |
| `echo $[VAR]` | Display variable value |
| `history` | Show command history |
| `alias [name]='[command]'` | Create command alias |
| `source [file]` | Execute script in current shell |
| `which [command]` | Show command location |
| `type [command]` | Display command type |

## File System and Mounting

| Command | Description |
|---------|-------------|
| `mount` | Show mounted filesystems |
| `sudo mount [device] [mountpoint]` | Mount filesystem |
| `sudo umount [mountpoint]` | Unmount filesystem |
| `fdisk -l` | List disk partitions |
| `lsof [file]` | List processes using file |
| `fuser [file]` | Show processes using file |

---

## Legend
- ⚠️ = Use with caution - can delete data or affect system
- **DANGEROUS** = Extremely destructive - double-check before using
- `[placeholder]` = Replace with actual value
- Commands requiring elevated privileges use `sudo`

## Quick Tips
- Use `Tab` for auto-completion
- Use `Ctrl+C` to cancel running command  
- Use `Ctrl+Z` to suspend command
- Use `!!` to repeat last command
- Use `!n` to repeat command number n from history
- Use `man [command]` to view manual page for any command