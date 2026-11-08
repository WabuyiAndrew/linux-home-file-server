## User and Group Management

A dedicated Linux group named `fileshare` is used to manage access to the shared directory.

The authorized Linux account is added to this group.

Samba maintains its own authentication database. The authorized Linux account is registered using the `smbpasswd` utility.

### Administration commands

- `whoami` — identifies the current user.
- `id` — displays user and group membership.
- `groupadd` — creates a Linux group.
- `usermod -aG` — adds a user to a supplementary group.
- `smbpasswd -a` — registers a Samba account.
- `smbpasswd -e` — enables a Samba account.
- `pdbedit -L` — lists Samba accounts.
- `pdbedit -Lv` - Lists more info about samba accounts

### Access control design

Access requires both Samba authorization and appropriate Linux filesystem permissions.
