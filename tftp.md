## How to create a tftp server in linux

```bash
sudo apt install tftpd-hpa -y

sudo vim /etc/default/tftpd-hpa 
  
  # /etc/default/tftpd-hpa

  TFTP_USERNAME="tftp"
  TFTP_DIRECTORY="/var/lib/blast"
  TFTP_ADDRESS=":69"
  TFTP_OPTIONS="--secure --create"

sudo systemctl restart tftpd-hpa.service 

sudo mkdir /var/lib/blast

sudo chmod -R 777 /var/lib/blast
sudo chown -R nobody:nogroup /var/lib/blast
```
