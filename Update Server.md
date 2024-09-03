# Updating Server Build with Git

## 1. Stop the Current Server Process
Before updating the server build, it's essential to stop the current server process to prevent conflicts or unexpected behavior.
```bash
pm2 stop 0
```

## 2. Run SteamCMD and login
Navigate to the directory where your server build is located. Assuming your server build is located in the /root/CAMPS-Server/Build/ directory:
```bash
steamcmd
login <username>
```

## 3. Update app
Get the latest update from Steam
```bash
app_update 2948910 validate
```
This command fetches the latest changes from the remote repository and merges them into your local branch.

## 4. Restart the Server Process
```bash
pm 2 start 0
```

Summary of Commands:
```bash
pm2 stop 0
steamcmd
login <username>
app_update 2948910 validate
pm 2 start 0
```
