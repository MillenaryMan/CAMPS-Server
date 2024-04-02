# To automatically run CAMPS server on startup, you can create a systemd service unit. (Ubuntu)

## 1. Create a systemd Service Unit File.
Open a terminal on your Ubuntu server.
```bash
sudo nano /etc/systemd/system/camps_server.service
```
## 2. Add the Service Configuration.
Inside the file, add the following lines:
```makefile
[Unit]
Description=CAMPS Server Service
After=network.target

[Service]
Type=simple
ExecStart=/root/CAMPS-Server/Build/CAMPS.x86_64 -batchmode -nographics -logfile /root/CAMPS-Server/logfile.log

[Install]
WantedBy=multi-user.target
```
After making the necessary changes, save and close the file by pressing Ctrl + X, then Y, and finally Enter.

## 3. Reload systemd and Enable the Service.
This reloads systemd to pick up the changes you made and enables the service to start automatically on each boot.
```bash
sudo systemctl daemon-reload
sudo systemctl enable camps_server
```
## That's it! :+1:  Your CAMPS server should now start automatically on boot.

  
> [!TIP]
> This command starts the service immediately.
```bash
sudo systemctl start camps_server
```
> [!TIP]
> To test if the service starts automatically on boot, you can reboot your server.
```bash
sudo reboot
```
> [!TIP]
> You can verify that it's running properly by checking its status.
```lua
sudo systemctl status camps_server
```
