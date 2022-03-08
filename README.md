# Installation

### For Arch users
It should work on other systems with systemd

```bash
makepkg -si             # install mbpfan executable and the service
systemctl start mbpfan  # start the service
pidof mbpfan            # check that is running
systemctl enable mbpfan # run the service on boot
```
