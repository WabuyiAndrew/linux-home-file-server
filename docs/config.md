## Installation Record

Samba and the SMB client utilities were installed on the Ubuntu Server using the APT package manager.

### Packages installed

- samba
- smbclient

### Verification commands

- `smbd --version`
- `smbclient --version`
- `systemctl status smbd`
- `systemctl is-enabled smbd`
- `testparm -s`

### Service management

The Samba service was enabled to start automatically during system boot.

### Configuration location

`/etc/samba/smb.conf`

### Implementation status

Samba installation and service verification completed.

### Inspect Samba's listening ports
sudo ss -u tulpn | grep -E ':(445|139)\b'

### Understand the logs
sudo journalctl -u smbd -n 30 --no-pager


