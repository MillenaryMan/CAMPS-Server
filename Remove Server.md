# Removing CAMPS-Server
## 1. Stop the CAMPS-Server Service
Before removing the CAMPS-Server directory, you need to stop the associated systemd service to prevent it from running.
```bash
sudo systemctl stop camps_server
```

## 2. Terminate the Current Server Process
Ensure that the CAMPS-Server process is terminated before proceeding.
- Check if the CAMPS-Server process is running
```bash
pgrep -f "CAMPS.x86_64"
```
- If the process is running, kill it
```bash
sudo pkill -f "CAMPS.x86_64"
```

## 3. Delete the CAMPS-Server Directory
Delete the CAMPS-Server directory using the rm command. Be cautious as this action is irreversible.
```bash
sudo rm -r /root/CAMPS-Server
```

## 4. Disable the CAMPS-Server Service
Disable the CAMPS-Server service to prevent it from starting automatically on boot.
```bash
sudo systemctl disable camps_server
```

## 5. Remove the CAMPS-Server Service
Finally, remove the systemd service file associated with the CAMPS-Server.
```bash
sudo rm /etc/systemd/system/camps_server.service
```

Summary of Commands:
```bash
# Stop the CAMPS-Server Service
sudo systemctl stop camps_server

# Terminate the Current Server Process
pgrep -f "CAMPS.x86_64"
sudo pkill -f "CAMPS.x86_64"

# Disable the CAMPS-Server Service
sudo systemctl disable camps_server

# Delete the CAMPS-Server Directory
sudo rm -r /root/CAMPS-Server

# Remove the CAMPS-Server Service
sudo rm /etc/systemd/system/camps_server.service
```
> [!NOTE]
> Double-check the paths and service names before executing the commands.
> Removing the CAMPS-Server directory and associated services is irreversible. Make sure you have backed up any necessary data before proceeding.
> You might need root or sudo privileges to execute these commands successfully.

By following these steps, you should be able to remove the CAMPS-Server from your server machine completely. 
If you have any questions or encounter any issues, feel free to ask in [discussions](https://github.com/MillenaryMan/CAMPS-Server/discussions).
