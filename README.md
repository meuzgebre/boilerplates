# Linux Commands Cheat Sheet

**Table of Contents**

* [Repositories](#repositories)
  * [Package Manager](#package-manager)
  * [Repository Manager](#repository-manager)
* [Navigation](#navigation)
  * [File System Navigation](#file-system-navigation)
  * [Directory Operations](#directory-operations)
* [File Management](#file-management)
  * [File Manipulation](#file-manipulation)
  * [File Permissions](#file-permissions)
* [Text Processing](#text-processing)
* [Process Management](#process-management)
    * [Viewing Processes](#viewing-processes)
    * [Managing Processes](#managing-processes)
* [System Information](#system-information)
  * [Hardware Information](#hardware-information)
  * [System Status](#system-status)
* [Network Management](#network-management)
* [User Management](#user-management)
    * [Users](#users)
    * [Group](#group)
* [Additional Resources](#additional-resources)

---

## Repositories

### Package Manager

**1.Installing Packages**

| Command                        | Description                      |
|--------------------------------|----------------------------------|
| `apt install <package>`        | Install a package using APT (Debian)  |
| `dnf install <package>`        | Install a package using DNF (RHEL)    |
| `pacman -S <package>`          | Install a package using Pacman (Arch) |

**2.Searching Packages**

| Command                        | Description                      |
|--------------------------------|----------------------------------|
| `apt search <keyword>`         | Searching a package using APT (Debian)  |
| `dnf search <keyword>`         | Searching a package using DNF (RHEL)    |
| `pacman -Ss <keyword>`         | Searching a package using Pacman (Arch) |

**3.Removing Packages**

| Command                        | Description                      |
|--------------------------------|----------------------------------|
| `apt remove <package>`         | Removing a package using APT (Debian)  |
| `dnf remove <package>`         | Removing a package using DNF (RHEL)    |
| `pacman -R <package>`          | Removing a package using Pacman (Arch) |


**Note**
  - while `apt-get` is still widely used and offers more fine-grained control, `apt` is generally preferred for its simplicity and better dependency management.
  - while `yum` is still functional and present in older RPM-based distributions, `dnf` is the preferred and recommended package manager for modern distributions


## Navigation

### File System Navigation

#### Basic Commands
- `cd [directory]`: Change directory.
- `pwd`: Print working directory.
- `ls`: List contents of current directory.
- `ls -l`: Detailed listing of contents.

#### Navigating Directories
- `cd ..`: Move up one directory.
- `cd ~`: Move to the home directory.
- `cd /`: Move to the root directory.

#### Absolute vs Relative Paths
- Absolute paths start from the root directory.
- Relative paths start from the current directory.

#### Tab Completion
- Press `Tab` to auto-complete file and directory names.

#### Hidden Files
- Hidden files start with a dot (e.g., `.gitignore`).
- Use `ls -a` to view hidden files.

### Directory Operations

#### Creating Directories
- `mkdir [directory]`: Create a new directory.

#### Removing Directories
- `rmdir [directory]`: Remove an empty directory.
- `rm -r [directory]`: Remove a directory and its contents.

#### Moving and Renaming Directories
- `mv [old directory] [new directory]`: Move or rename a directory.

#### Copying Directories
- `cp -r [source directory] [destination directory]`: Copy a directory and its contents.

#### Viewing Directory Contents
- `ls [directory]`: List contents of a specific directory.
- `ls -l [directory]`: Detailed listing of contents of a specific directory.

#### Changing Permissions
- `chmod [permissions] [directory]`: Change permissions of a directory.
