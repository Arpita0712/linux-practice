
**Learnt** how Linux manages file ownership, groups, and permissions, and how to control access using `chmod`, `chown`, and `chgrp`.

## Commands Learned

| Command | Purpose | Example |
|---------|---------|---------|
| `whoami` | Display current user | `whoami` |
| `id` | Show UID, GID, and groups | `id` |
| `groups` | List groups of current user | `groups` |
| `ls -l` | View file permissions and ownership | `ls -l` |
| `chmod` | Change file/directory permissions | `chmod 755 script.sh` |
| `chmod +x` | Make a file executable | `chmod +x script.sh` |
| `chown` | Change file owner | `sudo chown alice file.txt` |
| `chgrp` | Change file group | `sudo chgrp developers file.txt` |

## Key Learnings

- Every file has an **Owner**, **Group**, and **Others**.
- Linux permissions are represented as:
  - **Read (r) = 4**
  - **Write (w) = 2**
  - **Execute (x) = 1**
- `chmod` changes file and directory permissions.
- `chown` changes the file owner (and optionally the group).
- `chgrp` changes only the group ownership.
- `ls -l` displays permissions, owner, and group information.
- Common permission values:
  - **755** → Directories and executable scripts
  - **644** → Regular files
  - **600** → Private/sensitive files
- `-R` applies permission or ownership changes recursively.

## Quick Revision

| Permission | Meaning | Common Use |
|------------|---------|------------|
| `755` | `rwx r-x r-x` | Directories, scripts |
| `644` | `rw- r-- r--` | Regular files |
| `600` | `rw- --- ---` | Private files |
