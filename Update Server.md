# Updating CAMPS Server App

## 1. Stop the Current Server Process
Before updating the server build, it's essential to stop the current server process to prevent conflicts or unexpected behavior.
```bash
pm2 stop 0
```

## 2. Run SteamCMD and login
```bash
steamcmd
login <username>
```

## 3. Update app
Get the latest update from Steam
```bash
app_update 2948910
```

## 4. Restart the Server Process
```bash
pm 2 start 0
```

Summary of Commands:
```bash
pm2 stop 0
steamcmd
login <username>
app_update 2948910
pm 2 start 0
```
