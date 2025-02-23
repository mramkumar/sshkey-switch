# SSH-Switch

## Overview
SSH-Switch is a command-line utility that allows users to easily switch between multiple SSH keys. It automates the process of managing SSH keys by listing available keys, selecting one interactively, and adding it to the ssh-agent.

## Features
- Lists all valid SSH private keys from `~/.ssh/`
- Allows interactive selection of an SSH key
- Automatically starts `ssh-agent` if not running
- Removes previously added SSH keys before adding the new one
- Stores recently used keys for quick selection
- Provides instructions to activate the environment variables

## Installation
```sh
# 
```

## Usage
```sh
ssh-switch
```
Follow the on-screen instructions to select an SSH key.

## Example Output
```
Select SSH private key:
1) id_rsa
2) github_key
3) deploy_key
#? 2
✅ SSH key switched to: ~/.ssh/github_key
✅ ssh-agent is working correctly.
```

## Notes
- Ensure you run `source ~/.bashrc` if prompted to activate environment variables.
- The script only lists valid SSH private keys and excludes public keys or other files.

## License
This project is licensed under the MIT License.

