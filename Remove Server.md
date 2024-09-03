# Removing CAMPS-Server
## 1. Stop the CAMPS-Server Service
Before removing the CAMPS-Server directory, you need to stop the associated mp2 service.
```bash
mp2 stop 0
mp2 save
```

## 2. Delete the CAMPS-Server Directory
Delete the CAMPS-Server directory using the rm command. Be cautious as this action is irreversible.
```bash
sudo rm -rf /root/.local/share/Steam/steamapps/common/CAMPS-Server
```


Summary of Commands:
```bash
mp2 stop 0
mp2 save
sudo rm -rf /root/.local/share/Steam/steamapps/common/CAMPS-Server
```
> [!NOTE]
> Double-check the paths and service names before executing the commands.
> Removing the CAMPS-Server directory and associated services is irreversible. Make sure you have backed up any necessary data before proceeding.
> You might need root or sudo privileges to execute these commands successfully.

By following these steps, you should be able to remove the CAMPS-Server from your server machine completely. 
If you have any questions or encounter any issues, feel free to ask in [discussions](https://github.com/MillenaryMan/CAMPS-Server/discussions).
