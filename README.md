# VARS SSH Manager (vsm) ![](https://img.shields.io/maintenance/no/2016)

A CLI tool that helps manage SSH hosts. VSM keeps track of SSH hosts in a local repository file and allows you to quickly act on any stored host based on its assigned key.

## Features

You can:
- assign an SSH host to a key with optional cert file
- quickly SSH into a stored host by its key

## Commands

`vsm add <key> <host> <cert>`: Stores a new entry with specified key, SSH host, and optional certificate file path.

`vsm list`: Lists all current entries.

`vsm ssh <key_or_index>` Opens an SSH connection to the host referenced by the specified key or index.

`vsm remove <key_or_index>`: Removes a stored SSH host entry by its key or index.

See `vsm help` or simply `vsm` for a full list of commands with details.

## Usage

Clone this repo and symlink to `/usr/local/bin` (you may need `sudo` access)
```
git clone https://github.com/andrewscwei/vsm.git
sudo ln -s /path/to/vsm /usr/local/bin
```
