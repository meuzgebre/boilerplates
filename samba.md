## SMB SHARE

` sudo apt install samba -y `

` sudo mv smb.conf smb.conf.bak `

` sudo systemctl stop smbd.service `

` sudo vim smb.conf `

```
	workgroup = SHARE
	security = user
	map to guest = Bad User
	name resolve order = bcast host
	include = /etc/samba/shares.conf
```

` sudo vim shares.conf `

```
	[Public Files]
	path = /share/public_files
	force user = smbuser
	force group = smbgroup
	create mask = 0664
	force create mode = 0664
	directory mask = 0775
	force directory mode = 0775
	public = yes
	writable = yes

	[Protected Files]
	path = /share/protected_files
	force user = smbuser
	force group = smbgroup
	create mask = 0664
	force create mode = 0664
	directory mask = 0775
	force directory mode = 0775
	public = yes
	writable = no

```

` sudo mkdir -p /share/public_files `

` sudo mkdir -p /share/protected_files `

` sudo groupadd --system smbgroup `

` sudo useradd --system --no-create-home --group smbgroup -s /bin/false smbuser `

` sudo chown -R smbuser:smbgroup /share `

` sudo chmod -R g+w /share/ `

` sudo systemctl start smbd.service `
